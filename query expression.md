### Query Expression

1. **FROM:** from T
\[
$\frac{\{T\}}{\{T_1| T_1=T\}}$
\]

2. **SELECT:** select $T.\overline{\beta}$
\[
$\frac{\{T,\overline{\beta}\}}{\{T_1|T_1=\{\pi_{\overline{\beta}}(T)\}\}}$
\]

3. **WHERE:** where $\Theta$
\[
$\frac{\{T, \Theta\}}{\{T_1 | (\forall \alpha \in \sigma_\Theta (T), \alpha \in T_{1}) \wedge (\forall \alpha_1 \notin \sigma_{\Theta} (T), \alpha_1 \notin T_{1}) \wedge (\xi_{\alpha}(T)=\xi_{\alpha}(T_1))\}}$
\]
