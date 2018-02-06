
- http://blog.csdn.net/zuiwuyuan/article/details/48201655
- 学会了如何在Android studio项目中如何引用jar包后，那如何引用so文件呢？
它可不像Eclipse那样直接把so文件夹拷贝到libs文件夹下就好了。
总之，要引入so文件，你得注意下如何去配置：
  引入so文件：
  引入so文件也有两种方法，具体使用哪一种，看开发者自己如何选择了

  方法一：

     · 在“src/main”目录中新建名为“jniLibs”的目录；

     · 将so文件复制、粘贴到“jniLibs”目录内。
      注：如果没有引用so文件，可能会在程序执行的时候加载类库失败，有类似如下的DEBUG提示：
      java.lang.UnsatisfiedLinkError: Couldn't load library xxxx from loader dalvik.system.PathClassLoader