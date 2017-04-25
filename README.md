# awk
# awk学习随时补充
## 常用的awk内置函数：<br/>
    substr(s,1,6):截取s字段从第一个字符开始往后长度为6的子串并返回，注意awk中的str索引从1开始<br/>
    asort(a,b):仅对数组a的值进行排序，并把排序结果保存在b中，数组索引也是从1开始的<br/>
    asorti(a,b):对数组a的key进行排序，并把key的排序结果保存在数组b中，所以要在排序后取出每个key对应的值，需要从a中取：a[b[i]]<br/>
        asort()和asorti()函数俊辉返回原数组的长度：len = asort(a,b) / len = asorti(a,b)<br/>
        
## 几个tips:<br/>
    awk中的数组其实就是和python中的dict一样，实际上保存的是key-value对，所以它hi无序的，在对文本分析时，如果要求有序的操作，一定要调用asort()或 asorti()函数进行处理<br/>
    
    

