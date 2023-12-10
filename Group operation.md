1. GROUP BY
$$\frac{
\{T,\beta\}
}{
    \{T_{1}=(\overline{\beta},(\overline{\alpha_1},...,\overline{\alpha_k})) |\forall \overline{\alpha_i} \in\ (\overline{\alpha_1},...,\overline{\alpha_k}), 
 (\forall\ v_{ij}\ \in\ \pi_{\beta}(\overline{\alpha_i}),(v_{ij}=v_{i1})  \wedge(\forall\ v_{xy}\ \in \pi_{\beta}(\overline{\alpha_x}), (v_{ij}\ne v_{xy}),(x\in(1,...,k))\wedge(x\ne i)))   \wedge(\forall \alpha_x \in T,\xi_{\alpha_x}(T_1)=\xi_{\alpha_x}(T))
\wedge(\forall \alpha_y \in T_1,\xi_{\alpha_y}(T_1)=\xi_{\alpha_y}(T))\}
}$$

2. HAVING
$$\frac{
\{T,\Theta\}
}{
    \{T_1 | (\forall \alpha \in \sigma_\Theta (T),\alpha \in T_1) 
 \wedge(\forall \alpha_1 \notin \sigma_{\Theta} (T),\alpha_1 \notin T_1)\wedge(\xi_{\alpha}(T)=\xi_{\alpha}(T_1))\}
}$$

3. DISTINCT
$$\frac{
\{T,\beta\}
}{
    \{T_{1} | (\forall \alpha \in T,\ \xi_{\alpha} (T_1)=1) 
 \wedge(\forall \alpha_1 \in T_1,\ \alpha_1 \in T )\}
}$$

4. ORDER BY
$$\frac{
\{T,\beta\}
}{
    \{T_{1} | (\forall \alpha \in T_1,\ \xi_{\alpha} (T_1)=\xi_{\alpha} (T)) 
\wedge(\forall \alpha \in T,\ \xi_{\alpha} (T)=\xi_{\alpha} (T_1))\\
 \wedge(\forall \alpha_i \in \sigma_{T_1.{\overline{\beta}}}(T_1),\ \alpha_i > \alpha_{i+1} )\}
}$$













