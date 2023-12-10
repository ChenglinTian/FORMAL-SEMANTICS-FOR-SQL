1. UNION
$$\frac{
    \{T_{1}, T_{2}\}
}{
    \{T | (\forall \alpha_{1} \in T_1,\forall \alpha_{2} \in T_2, \alpha_{1} , \alpha_{2} \in T) \wedge(\forall \alpha \in T, (\xi_{\alpha}(T)=1)\wedge((\alpha \in T_1)\vee(\alpha \in T_2)))\}
}$$

2. INTERSECT
$$\frac{
    \{T_{1}, T_{2}\}
}{
    \{T | ((\forall \alpha \in T_1, ((\alpha  \in T_2) \wedge (\alpha  \in T)) \vee ((\alpha  \notin  T) \wedge (\alpha  \notin T_2))) \wedge ((\forall \alpha \in T_2, ((\alpha  \in T_1) \wedge (\alpha  \in T)) \vee  ((\alpha  \notin  T) \wedge (\alpha  \notin T_1))) \wedge (\forall \alpha \in T, (\xi_{\alpha}(T)=1)\wedge((\alpha \in T_1)\wedge(\alpha \in T_2)))\}
}$$
 
3. EXCEPT
$$\frac{
    \{T_{1}, T_{2}\}
}{
    \{T | (\forall \alpha \in T_1, ((\alpha  \in T) \wedge (\alpha  \notin T_2) \vee ((\alpha  \notin T) \wedge (\alpha  \in T_2))) \wedge (\forall \alpha \in T,(\alpha \in T_1) \wedge (\xi_{\alpha}(T)=1))\}
}$$
 
4. UNION ALL
$$\frac{
    \{T_{1}, T_{2}\}
}{
    \{T | (\forall \alpha_{1} \in T_1,\forall \alpha_{2} \in T_2, \alpha_{1} , \alpha_{2} \in T) \wedge(\forall \alpha \in T, (\alpha \in T_1) \vee(\alpha \in T_2)) \wedge (\forall \alpha \in T, \xi_{\alpha}(T)=\xi_{\alpha}(T_1)+\xi_{\alpha}(T_2))\}
}$$ 

5. INTERSECT ALL
$$\frac{
    \{T_{1}, T_{2}\}
}{
    \{T | (\forall \alpha \in T_1, ((\alpha  \in T_2) \wedge (\alpha  \in T) \vee ((\alpha  \notin T) \wedge (\alpha  \notin T_2)))) \wedge(\forall \alpha \in T_2, ((\alpha  \in T_1) \wedge (\alpha  \in T) \vee ((\alpha  \notin T) \wedge (\alpha  \notin T_1)))) \wedge (\forall \alpha \in T,\ \xi_{\alpha}(T)=min(\xi_{\alpha}(T_1),\xi_{\alpha}(T_2)))\}
}$$   

6. EXCEPT ALL
$$\frac{
    \{T_{1}, T_{2}\}
}{
    \{T | (\forall \alpha \in T_1, ((\alpha  \in T) \wedge (\alpha  \notin T_2) \vee ((\alpha  \notin T) \wedge  (\alpha  \in T_2)))) \wedge (\forall \alpha \in T, \xi_{\alpha}(T) = max(\xi_{\alpha}(T_1)-\xi_{\alpha}(T_2)),0)\}
}$$
