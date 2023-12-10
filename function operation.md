1. RTRIM
$$\frac{
\{str\}
}{
    \{str1 | (str1=str[0,len(str1)]) \wedge (\forall i \in (len(str1),len(str)),str[i]=space) \}
}$$

2. LTRIM
$$\frac{
\{str\}
}{
   \{str1 | (str1=str[len(str)-len(str1),len(str)]) \wedge (\forall i \in (0,len(str)-len(str1)),str[i]=space) \}
}$$

3. RPAD
$$\frac{
\{str,length,str1\}
}{
   \{str2 | (len(str2)=length)  \wedge (str2[0,len(str)]=str) \wedge (\forall i \in (len(str),len(str2)), str2[i]=str1[(i-len(str)) mod (len(str1))]) \}
}$$

4. LPAD
$$\frac{
\{str,length,str1\}
}{
   \{str2 | (len(str2)=length) \wedge(str2[len(str2)-len(str),len(str2)] =str) \wedge(\forall i \in (0,len(str2)-len(str),str2[i]=str1[(i)mod(len(str1))]) \}
}$$

5. RIGHT
$$\frac{
\{str,length\}
}{
   \{str1 | str1=str[len(str)-length,len(str)] \}
}$$

6. LEFT
$$\frac{
\{str,length\}
}{
   \{str1 | str1=str[0,length]\}
}$$

7. INSTR
$$\frac{
\{str,str1\}
}{
   \{n | str2=str1[n,n+len(str2)]\wedge(\forall i \in (0,n-1),str1[i,i+len(str2)]\ne str2\}
}$$

8. LOCATE
$$\frac{
\{str1,str2,start\}
}{
   \{n | str1=str2[n,n+len(str1)]\wedge(\forall i \in (start,n),str2[i,i+len(str1)]\ne str1\}
}$$

9. POSITION
$$\frac{
\{str1,str2,start\}
}{
   \{n | str1=str2[n,n+len(str1)]\wedge(\forall i \in (start,n),str2[i,i+len(str1)]\ne str1\}
}$$


10. SUBSTR
$$\frac{
\{str,start,length\}
}{
   \{str1 | (str1=str[start,start+length]) \wedge(\forall i \in (start,n),str2[i,i+len(str1)]\ne str1\}
}$$

11. SUBSTRING
$$\frac{
\{str,start,length\}
}{
   \{str1 | (str1=str[start,start+length]) \wedge(\forall i \in (start,n),str2[i,i+len(str1)]\ne str1\}
}$$

12. MID
$$\frac{
\{str,start,length\}
}{
   \{str1 | (str1=str[start,start+length]) \wedge(\forall i \in (start,n),str2[i,i+len(str1)]\ne str1\}
}$$

13. SUBSTRING INDEX
$$\frac{
\{str,char,index\}
}{
   \{str1 | str1=str[0,len(str1)]\wedge(str[len(str1)]=index \wedge(\xi_{char}(str)=index-1\}\\
}$$

14. REVERSE
$$\frac{
\{str1\}
}{
   \{str1 | (len(str1)=len(str))\wedge(\forall i \in (0,len(str)),str[i]=str1[len(str1)-i])\}
}$$

15. INSERT
$$\frac{
\{str,start,length,str1\}
}{
   \{str2 | (str2[0,start]=str[0,start]) \wedge (str2[start+len(str1),len(str2)]=str[start+length,len(str2)])\wedge(str2[start,start+len(str1)]=str1\wedge(len(str2)-len(str1=len(str)-length)\}
}$$

16. FIELD
$$\frac{
\{str,\overline{str}\}
}{
   \{n | (\overline{str}[n]=str) \wedge(\forall i \in (0,n),\overline{str} \ne str)\}
}$$

17. FIND IN SET
$$\frac{
\{str,\overline{str}\}
}{
   \{n | (\overline{str}[n]=str) \wedge(\forall i \in (0,n),\overline{str} \ne str)\}
}$$

18. ELT
$$\frac{
\{index,\overline{str}\}
}{
   \{str | (\overline{str}[index]=str)\wedge(\forall i \in (0,index),\overline{str}[i]\ne str)\}
}$$


19. SPACE
$$\frac{
\{n\}
}{
   \{str | (len(str)=n)\wedge(\forall i \in (0,len(str)),str[i]=space)\}
}$$

20. REPEAT
$$\frac{
\{str,n\}
}{
   \{str1 | (len(str1)=n*len(str))\wedge(\forall i \in (0,len(str1)),str1[i]=str[(i)mod(len(str))])\}
}$$

21. UPPER
$$\frac{
\{str\}
}{
   \{str | (len(str)=len(str1))\wedge(\forall i \in (0,len(str)),str1[i]=ascii(str[i]-32))\}
}$$

22. UCASE
$$\frac{
\{str\}
}{
   \{str | (len(str)=len(str1))\wedge(\forall i \in (0,len(str)),str1[i]=ascii(str[i]-32))\}
}$$

23. LOWER
$$\frac{
\{str\}
}{
   \{str | (len(str)=len(str1))\wedge(\forall i \in (0,len(str)),str1[i]=ascii(str[i]+32))\}
}$$

24. LCASE
$$\frac{
\{str\}
}{
   \{str | (len(str)=len(str1))\wedge(\forall i \in (0,len(str)),str1[i]=ascii(str[i]+32))\}
}$$

25. ASCII
$$\frac{
\{char\}
}{
   \{n | n=char+0\}
}$$

26. CHAR
$$\frac{
\{n\}
}{
   \{char | char=ascii(n)\}
}$$

27. CASE
$$\frac{
\{\Theta,\Theta_{1},\Theta_{2}\}
}{
   \{\Theta_{3} | \Theta_{3}=\Theta_{1}, \Theta=TRUE; \Theta_{3}=\Theta_{2}, \Theta=FALSE\}
}$$

28. IF
$$\frac{
\{\Theta,\Theta_{1},\Theta_{2}\}
}{
   \{\Theta_{3} | \Theta_{3}=\Theta_{1}, \Theta=TRUE; \Theta_{3}=\Theta_{2}, \Theta=FALSE\}
}$$

29. NULLIF
$$\frac{
\{\Theta_{1},\Theta_{2}\}
}{
   \{\Theta_{3} | \Theta_{3}=NULL, \Theta_{1}=\Theta_{2}; \Theta_{3}=\Theta_{1}, \Theta_{1}\ne \Theta_{2} \}
}$$

30. COALESCE
$$\frac{
\{\overline{str}\}
}{
   \{n | (\overline{str}[n]=NULL) \wedge(\forall i \in (0,n),\overline{str}\ne NULL)\}
}$$

















