CQ1: $T.\beta$ FROM T

$$
\frac{T \text{ FROM } T, T \text{ SELECT } \beta \{\pi_{\beta}(T)\}}{T \text{ FROM; SELECT } \beta \{\pi_{\beta}(T)\}}
$$

CQ2: SELECT $T_1.\overline{\beta}$ FROM $T\_1$ Join Operation $T\_2$

$$
\frac{T_1, T_2 \text{ JOIN Operation } T, T \text{ FROM } T, T \text{ SELECT } \beta \{\pi_{\beta}(T)\}}{T_1, T_2 \text{ JOIN Operation; FROM; SELECT } \beta \{\pi_{\beta}(T)\}}
$$

CQ3: SELECT $T.\overline{\beta}$ FROM T WHERE $\Theta$

$$
\frac{T \text{ FROM } T, T \text{ WHERE } \Theta \{\sigma_{\Theta}(T)\}, \{\sigma_{\Theta}(T)\} \text{ SELECT } \beta \{\pi_{\beta}(\sigma_{\Theta}(T))\}}
{T \text{ FROM; WHERE } \Theta; \text{ SELECT } \beta \{\pi_{\beta}(\sigma_{\Theta}(T))\}}
$$

CQ4: SELECT Aggregation Operation ($T.\beta$) FROM T

$$
\frac{\{T\} \text{ FROM } \{T\}, \{T, \beta\} \text{ Agg } \{x_{agg}\}, \{T, x_{agg}\} \text{ SELECT } \{\pi_{x_{agg}}(T)\}}
{\{T, \beta\} \text{ FROM; Aggregation Operation } (T.\beta); \text{ SELECT } \{\pi_{x_{agg}}(T)\}}
$$

CQ5: SELECT $\beta$ FROM T GROUP BY $\beta$ HAVING $\Theta$

$$
\frac{\{T\} \text{ FROM } \{T\}, \{T\} \text{ GroupBy } \{T_1\}, \{T\} \text{ HAVING } \Theta \{\sigma_{\Theta}(T)\}, \{\sigma_{\Theta}(T)\} \text{ SELECT } \beta \{\pi_{\beta}(\sigma_{\Theta}(T))\}}
{\{T, \beta\} \text{ FROM; GroupBy; HAVING } \Theta; \text{ SELECT } \beta \{\pi_{\beta}(\sigma_{\Theta}(T))\}}
$$

CQ6: SELECT $T.\beta_1$ FROM T ORDER BY $\beta_1$ ASC/DESC

$$
\frac{\{T\} \text{ FROM } \{T\}, \{T, \beta_1\} \text{ SELECT } \{\pi_{\beta_1}(T)\}, \{\pi_{\beta_1}(T)\} \text{ ORDER BY } \{\beta_1 \text{ ASC/DESC}\}}{\{T, \beta_1\} \text{ FROM; SELECT; ORDER BY } \{\beta_1 \text{ ASC/DESC}\}}
$$

CQ7: \( \text{CQ\$1\_1\$} \) Collection Operation \( \text{CQ\$1\_2\$} \)

$$
\frac{\{T_1, \overline{\beta_1}\} \text{CQ\$1\_1\$} \{\pi_{\overline{\beta_1}}(T_1)\}, \{T_2, \overline{\beta_2}\} \text{CQ\$1\_2\$} \{\pi_{\overline{\beta_2}}(T_2)\}, \{T_1, T_2\} \text{Collection Operation} \{T\}}{\{T_1, T_2\} \text{CQ\$1\_1\$; CQ\$1\_2\$; Collection Operation;} \{T\}}
$$








