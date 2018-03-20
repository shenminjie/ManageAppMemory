# 日常记录
# 如何管理应用内存

## 使用Android Profiler进行查看使用内存的情况
<p> 使用ComponentCallbacks2进行监听各大组件内存情况，及时释放资源（Activity，Application,Service,ContentProvider）</p>

## 使用更高效的代码
### 谨慎使用service，如若使用及时释放资源,建议使用IntentService
### 使用优化过的数据集合,避免使用在移动设备未经优化过的集合，如HashMap.HashMap会产生多余的内存，建议使用android提供的SparseArray,SparseArray更高效，避免了装箱过程中产生多余的内存
### 谨慎使用抽象，虽然使用抽象能使代码更灵活并且更好的后期维护，但是使用抽象执行过程中会占用更多的ram。如果抽象不能给你的代码带来好处，建议避免使用抽象

## 去除额外的资源以及引入包
### 优化你APK的大小
### 使用Dagger2来管理你的依赖
### 谨慎使用三方的依赖包，有的三方工具是好用，但可能不是为移动端设计的，如若使用需要通过优化。



https://developer.android.google.cn/topic/performance/memory.html#code









