## 任务一
1.	用plantuml画出example的类图与Scene中main方法执行过程中的对象时序图
![](http://www.plantuml.com/plantuml/png/hLFDZXCn3BxtANBCGli2BOTb9RINFI0Mk20EQMkc4Pbab3Z0KdXtFB4pdKm12Oazx3Ysu-ydxcr24p7tRcKzGlna3g0UGwHGdLUA_hu4UrGkcAEcXWyV5JZemMEwsLtAYIveIJnYjBvJ7U1hP_oO_RcQpNwmtkmTp8SdQWt9eWrUrq0D4iZKAT_DcgL6myVqU-Co2Dx1cPJKNTuJ5AjXl0rhC3i-2TU1YEwknIeZ01kc-TKC-bzKYuqlVcms3PLAxnxW-qGieK5xa9p24t34qziYWRojTLqfBew2dSfdrtZD9Trqj2gSzV1kq0_qAV5DOnVvDvYOe0YTETYO1T_Wa15gFI4CnHEckTqoh7f6rbHJNldSg_kGu_7oLYgkk_LU1b_j1kVB5H4kJd5kDAe4TqzlZF-iopmAfBKU5q-8WGDE_wSLdHPeAZ13umEU8FvnaUNNmZjKhgpA_-ssWXSBwzIwMNGDpgrfuwj9c0fQQIgUEF0TdkPCXuowGZl-hWixArsrI6mrv__geRGJ1mmlOpHFapguA4c_bLBF8cV1gdL-oNdnWbAzxX8gwlaS_nRyCVVk5m00)

![](http://www.plantuml.com/plantuml/png/LK-x3i8m3Dpp5VS3dP4wL1KB2mCINv0sfaHAayXs1lXw4WKXElWXt_dEdaKjQzc3iQicXZxfGlGcXiaLyAlFDYgkFj9X88cLs9W635FB8sv5SSAM2Zk1ZqqBeIrsyZ3rEa98iR-4mWDMS2xB4kZ-5VmTSAJt_X_jdaqV9SD6XrpzKusGDZDJTFMh3m00)


2.	尝试从面向对象编程角度理解`example`的设计理念，具体阐述这样写的好处与可改进之处（越详细越好）

	好处：
	将sorter Linable作为接口给gourd 和 geezer使用。以便于在更换sorter的实现方法和Linable 的存储方式等时可以不用额外更改其他类的代码。
	Position作为Line的内部类，可以允许Line中positions的各项采取不同的Linable实现类。
	可改进之处：
	可以将Gourd也改进为类，这样便于gourd的创建和维护。