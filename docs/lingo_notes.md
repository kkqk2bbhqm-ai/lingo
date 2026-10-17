# LINGO 学习笔记
## 基础语法框架
sets:
! 集合定义；
endsets
data:
! 数据赋值；
enddata
! 表达式与目标、约束；
end

### 集合
1. 文本集合：`set1/A,B,C/: X,Y;`
2. 下标数字集合：`years/1..5/: capacity;`

### Data段规则
- 写数值：代表固定已知参数
- 不赋值：变量，LINGO求解，默认 ≥0

### 内置函数
- `@abs(x)`：取绝对值
- `@smin(a,b,c...)`：取最小值
- `@smax(a,b,c...)`：取最大值
- `@free(x)`：取消变量非负限制
- `@bnd(low, x, high)`：设置变量上下界

### 常见报错
Error 11：语法错误，大概率中文标点符号，LINGO只认英文符号。
