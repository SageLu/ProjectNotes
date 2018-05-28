## Intent ##

###隐式 Intent 示例###

[隐式 Intent 验证](https://developer.android.google.cn/guide/components/intents-filters.html)

	//Create the text message with a string
	Intent sendIntent = new Intent();
	sendIntent.setAction(Intent.ACTION_SEND);
	sendIntent.putExtra(Intent.EXTRA_TEXT, textMessage);
	sendIntent.setType("text/plain");
	//隐式意图需要验证
	// Verify that the intent will resolve to an activity

	if (sendIntent.resolveActivity(getPackageManager()) != null) {
    startActivity(sendIntent);
	}
###Intent的跳转添加title，用于描述，跳转的意图是干嘛用的###
	Intent intent = new Intent();
    intent.setType("image/*");
    intent.setAction(Intent.ACTION_GET_CONTENT);
    intent.addCategory(Intent.CATEGORY_OPENABLE);
    startActivityForResult(
		Intent.createChooser(intent, "SelectPicture"), 
							REQUEST_SELECT_PICTURE);
##图片裁剪的适配7.0前后的比较（参考Android API19 和 API27）##
###android   api27  8.1###
(1)选择系统相册的某一张照片的uri :  
**Uri albumUri==**
	 content://com.android.providers.media.documents/document/image%3A1310

(2)选择系统相册的某一张照片的path :  
**File albumPath==**
	/storage/emulated/0/20180122062942.png

(3)Build.VERSION_CODES.N（24）大于等于Android7.0 根据上边的path获取的uri：
  （这个是输入的Uri） intent.setDataAndType(sourceUri, "image/*");

**Uri sourceUri==** 
	`content:`//media/external/images/media/1310

(4)自己定义的一个File 

**File  cropFile==** 
/storage/emulated/0/Android/data/com.zzhl.luluphotopicker/cache/2018-02-05-01-29-23-1-1517812163551.jpg

(5)根据自己定义的cropFile转换成Uri ,即裁剪生成的Uri 
   （这个是输出的Uri）## intent.putExtra(MediaStore.EXTRA_OUTPUT, cropUri);
**Uri cropUri==**
	 file:///storage/emulated/0/Android/data/com.zzhl.luluphotopicker/cache/2018-02-05-01-29-23-1-1517812163551.jpg



###android   api19  4.4###
**Uri albumUri==**
	 content://com.android.providers.media.documents/document/image%3A975

**File albumPath==**
	 /storage/emulated/0/PhotoNoter/intro_md.jpg

**Uri sourceUri==** 
	`file:`///storage/emulated/0/PhotoNoter/intro_md.jpg

**File  cropFile==** 
	/storage/emulated/0/Android/data/com.zzhl.luluphotopicker/cache/2018-02-05-14-35-17-1-1517812517214.jpg

**Uri cropUri==**
	 file:///storage/emulated/0/Android/data/com.zzhl.luluphotopicker/cache/2018-02-05-14-35-17-1-1517812517214.jpg



**总结：不同之处在于sourceUri 的类型不一样，一个为content ,一个为file.**