# 18、leetcode709. 转换成小写字母
解法一：
--  
代码： 
--
<pre>
/**
 * @author lihe
 * @date 2019/10/18 12:12
 * @descriptor  709. 转换成小写字母
 */
public class ToLowerCase_709 {
    public static String toLowerCase(String str) {
        StringBuilder builder = new StringBuilder();
        for (char c:str.toCharArray()) {
            if(c >= 'A' && c <= 'Z'){
                builder.append((char)(c+32));
            }else
                builder.append(c);
        }
        return builder.toString();
    }
    public static void main(String[] args) {
        String s = "Hello";
        String s1 = toLowerCase(s);
        System.out.println(s1);
    }
}
</pre>
