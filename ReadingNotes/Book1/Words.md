## 名词含义

* **字面量**：字面量就是指这个量本身，比如字面量3。也就是指3. 再比如 string类型的字面量"ABC", 这个"ABC" 通过字来描述。 所以就是字面量，虽然很难下定义。 你就理解成一眼就能知道的量。 对比下 string x; 那么x 是多少呢？ 它是个变量，你不确定它的值。 但是string x="ABC"， 你当然知道"ABC" 就是"ABC"了，一眼就能看到值的量（有点像常量）。 string x="ABC" 意思是把字面量"ABC" 赋值给变量X. 再举例 const string y="cbd". 意思是把字面量"cbd" 赋值给了常量y. 明白了吧？ 总之就是描述自己的量。 "ABC" 它描述了自己，你看到了就知道它是"ABC"了。
* **符号引用**：符号引用以一组符号来描述所引用的目标，符号可以是任何形式的字面量，只要使用时能无歧义地定位到目标即可。符号引用与虚拟机实现的内存布局无关，引用的目标并不一定已经加载到内存中。各种虚拟机实现的内存布局可以各不相同，但是他们能接受的符号引用必须都是一致的，因为符号引用的字面量形式明确定义在Java虚拟机规范的Class文件格式中。
* **直接引用**：直接引用可以是直接指向目标的指针、相对偏移量或是一个能间接定位到目标的句柄。直接引用是和虚拟机实现的内存布局相关的，同一个符号引用在不同虚拟机实例上翻译出来的直接引用一般不会相同。如果有了直接引用，那引用的目标必定已经在内存中存在。
* **全限定名**：类名全称，带包路径，将"."替换为"/"。如"java/lang/String"
* **非虚方法**：invokestatic指令调用的静态方法，invokespecial调用的实例构造器、私有方法和父类方法，这4类方法能在解析阶段确定唯一调用版本，在类加载阶段会把符号引用解析为该方法的直接引用，这类方法称为非虚方法。final虽然被invokevirtual指令调用，但由于无法覆盖，也是非虚方法。
* **虚方法**：invokevirtual调用所有的虚方法（final修饰除外）。除了非虚方法，都是虚方法。
* **方法签名**：
* **引用**：如果reference类型的数据中存储的数值代表的时另外一块内存的起始地址，就成为这块内存代表着一个引用。



## 知识点

* 数组是对象？
* 对象的属性是什么？