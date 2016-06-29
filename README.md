# SortRichEditor

支持图片文字混合编辑、排序的富文本编辑器

目前暂时支持的功能：

 - 支持图片文字混合添加、修改、删除
 - 支持文字中间随意插入一张或多张图片
 - 支持图片文字任意排序


# Preview

<img src="preview/SortRichEditor.gif"/>


# Usage

目前没有做很好的封装，如果需要使用SortRichEditor，请copy以下文件到您的工程中 <br/>
- SortRichEditor.java
- DataImageView.java
- DeletableEditText.java
- shape_dash_edit.xml
- icon_add_text.png (xhdpi)
- icon_delete.png (xhdpi)

copy完成后，在布局文件中
```
    <com.hitomi.sortricheditor.view.editor.SortRichEditor
        android:id="@+id/richEditor"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:background="#fff" />
```
SortRichEditor不包含照片墙、选择照片插入照片、拍照插入等功能，SortRichEditor只提供可插入图片的方法
如果需要以上功能，可以参照本项目其他代码。以后会将这些功能组件封装在里面。


# TODO

- [x] 图片压缩问题防止OOM
- [ ] 优化插入图片的速度
- [ ] 点击图片预览功能
- [x] 优化软键盘的显示和隐藏
- [ ] 排序操作方式改写为长按图片即可排序
- [ ] 重构SortRichEditor类

