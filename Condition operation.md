1. EXISTS
$$\frac{
\{\Theta \}
}{
    \{\Theta_1 | \Theta_1=(\Theta = TRUE)\}
}$$

2. AND
$$\frac{
\{\Theta_{1}, \Theta_{2}\}
}{
    \{\Theta |  \Theta=\Theta_{1} \wedge \Theta_{2} \}
}
$$

3. OR
$$\frac{
\{\Theta_{1}, \Theta_{2}\}
}{
    \{\Theta |  \Theta=\Theta_{1} \vee \Theta_{2} \}
}$$

4. NOT
$$\frac{
\{\Theta_{1}\}
}{
    \{\Theta |  \Theta = \neg \Theta_{1}\}
}
$$

5. IS NULL
$$\frac{
\{\Theta\}
}{
    \{\Theta_1 |  \Theta_1 = (\Theta = NULL)\}
}$$

6. IS NOT NULL
$$\frac{
\{\Theta\}
}{
    \{\Theta_1 |  \Theta_1 = (\Theta \ne NULL)\}
}$$

7. BETWEEN
$$\frac{
\{T,\beta,value_1,value_2\}
}{
    \{\Theta |  \Theta=(v \in \pi_{\beta}(T),(v \ge value1) \wedge (v \le value2))\}
}$$


