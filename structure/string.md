
字符串.txt


字符串去重
	可以问面试官是ascll 还是 unicode



字符串匹配问题
	1.暴力法
		暴力法胜在容易理解，代码也很简便。主要思路是将匹配字符串p和s进行一对一进行比较
		直到找到匹配字符串

	Rabinkarp(hash 滚动hash)
		通过计算每个n大小的字符串计算其hash值，然后匹配其hsah只需要O(1)的时间复杂度。
		但是由于预处理的时间为(O(m*n))所以还需要进行优化。
		后来有位大牛提出了一个滚动hash的优化思路。
		其实就是在计算第一个hash源字符串之后，向前推进一位的同时，扣除最后一位，得到新的字符串
		hash值，这样在预处理字符串的hash值只需要O(m+n) m是源字符串所花费的时间，n是匹配字符串所花费的时间。最后进行m次比较hash值则可以找出所有匹配的字符串位置


	kmp```