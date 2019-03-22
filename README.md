# Chinese-Std-GB-T-7714-2005-numeric-Chinese
--------------------------
## 介绍
* 本CSL文件部分实现了`GB/T 7714-2005 文后参考文献著录规则`的内容，参考文献表采用`顺序编码制`
* 适配软件为`Zotero 4.0.29.17`，其他版本未测试
## 关于Zotero的使用
* Title部分应该包含“题名: 其他题名信息”
* Title必然存在，Author不一定存在
* Edition处需要完整添加“新1版”、“5th ed.”等字样（而不是仅提供阿拉伯数字之类的，因为并不是所有版本号都是“第x版”的形式）
* Place：无出版地的中文文献著录“出版地不详”，外文文献著录“S.l.”，并置于方括号内
* Publisher：无出版者的中文文献著录“出版者不详”，外文文献著录“s.n."，并置于方括号内
* 支持的著录项目包括：专著、专著中的析出文献、连续出版物中的析出文献、专利、电子文献
* Zotero中的Computer Program文献类型：在使用时文献标志代码会标注为[M]，需注意
* Zotero中的Patent文献类型：把Country（即“专利国别”）信息复制入“Extra”中
* 在使用Word附加组件生成文后参考文献列表时，Document Preferences中的Language建议设置为English，以使责任者数量大于3时显示为“, et al”（若设置为中文，显示为“等”而不是“, 等”）
## 关于实现`GB/T 7714-2005`时的一些约定
* 其他责任者仅包括译者，并在所有人名列表后加“, 译”
* 电子文献：除“引用日期”外，略去“出版项”信息，即无“出版地”、“出版者”、“出版年”、“更新或修改日期”信息
* chinese-std-gb-t-7714-2005-numeric-chinese-yet-another-implementation-without-access-date-and-url：对于非“电子文献”类型的著录项目，取消其“引用日期”与“获取和访问路径”信息
## 存在的问题
* Journal Article的URL有时不在参考文献列表中显示
* 若文献的某一项（如Author）空缺，分隔符的处理不一定合规
## 文档
* 文后参考文献csl编写.xlsx：记录了支持的著录格式、文献类型及其他
* 文后参考文献csl编写.xmind：XMind文件，记录了一些编写时的零碎
## 关于多作者的“等”、“et al”问题
* 感谢@specter119 在issue中提到的方案，参考https://zhuanlan.zhihu.com/p/53594081
