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
