1. NATURAL JOIN
$$\frac{
\{T_{1}, T_{2}\}
}{
\{T | 
 \forall \alpha \in \pi_{T.{\overline{\beta}}}(T),(\alpha \in \pi_{T_1.{\overline{\beta}}}(T_1))\wedge(\alpha \in \pi_{T_2.{\overline{\beta}}}(T_2)) \wedge(\xi_{\alpha}(T)=1)\} 
}$$

2. LEFT JOIN
$$\frac{
\{T_{1}, T_{2}\}
}{
\{T | 
 (\forall \alpha \in \pi_{T_1.{\overline{\beta}}}(T),\alpha \in \pi_{T_1.{\overline{\beta}}}(T_1),\xi_{\alpha}(T)=1) \wedge(\forall \alpha \in \pi_{T_2.{\overline{\beta}}}(T),\alpha \in \pi_{T_2.{\overline{\beta}}}(T_2),\xi_{\alpha}(T)=1) \}
}$$

3. RIGHT JOIN
$$\frac{
\{T_{1}, T_{2}\}
}{
\{T | 
 (\forall \alpha \in \pi_{T_1.{\overline{\beta}}}(T),\alpha \in \pi_{T_1.{\overline{\beta}}}(T_1),\xi_{\alpha}(T)=1) \wedge(\forall \alpha \in \pi_{T_2.{\overline{\beta}}}(T),\alpha \in \pi_{T_2.{\overline{\beta}}}(T_2),\xi_{\alpha}(T)=1) \}
}$$

4. FULL JOIN
$$\frac{
\{T_{1}, T_{2}\}
}{
\{T | 
 (\forall \alpha \in \sigma_{T_1.{\overline{\beta}}}(T),\alpha \in \sigma_{T_1.{\overline{\beta}}}(T_1),\xi_{\alpha}(T)=1)\wedge(\forall \alpha \in \sigma_{T_2.{\overline{\beta}}}(T),\alpha \in \sigma_{T_2.{\overline{\beta}}}(T_2),\xi_{\alpha}(T)=1) \}
}$$

5. ON
$$\frac{
\{T,\Theta\}
}{
\{T_1 | (\forall \alpha \in \sigma_\Theta (T),\alpha \in T_{1}) \wedge(\forall \alpha_1 \notin \sigma_{\Theta} (T),\alpha_1 \notin T_{1})\wedge(\xi_{\alpha}(T)=\xi_{\alpha}(T_1))\}
}$$












