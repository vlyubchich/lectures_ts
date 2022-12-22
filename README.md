Todo
- check presence of comments "<!--" in QMD files to fix that.
- check comments from past PDFs to fix typos
- check that all labels # are cited (figures, tables)
- check grammar
- check :: and library() calls and add packages to the software list
- add an empty line between :| and code or comments in each chunk
- in Trend tests, add Chapter~8 of \citet{Chatterjee:Hadi:2006} and Chapter~5 of \citet{Chatterjee:Simonoff:2013} about the effects of autocorrelation.
- add that tsa::arimax is a tranfrer function, not ARIMAX model
- add a section on panel data analysis
- use "we" not "you" in lectures

# Format

Replace  
\bm with \boldsymbol    
Figure~\ref{fig: with @fig-
\begin{equation} with $$
\end{equation}
\citet{ with @
vs.\ with vs. 

a.k.a.
changepoint
nonlinear
nonparametric
homoscedasticity
heteroscedasticity
$p$-value
$\mathrm{WN}(0,s^2)$ -- have WN in math env

**Objectives**

**Reading materials**

in bold. Use *italics* for highlights in text.

Use 'single quotes' whenever possible.

Space and capital letter after a comment sign: # This is a comment

Cite
@Brockwell:Davis:2002
or
[@Brockwell:Davis:2002]
or
[@Rebane:Pearl:1987;@Pearl:2009]

Recall the classical decomposition
$$
Y_t = M_t + S_t + \epsilon_t,
$${#eq-trseas}

model as @eq-trseas is

```{r}
#| label: fig-shampoo
#| fig-cap: "Monthly shampoo sales over three years and a corresponding sample ACF."

p1 <- autoplot(shampoo) +
    xlab("Year") +
    ylab("Sales") +
    theme_light()
p2 <- forecast::ggAcf(shampoo) +
    ggtitle("") +
    xlab("Lag (months)") +
    theme_light()
p1 + p2 +
    plot_annotation(tag_levels = 'A')
```

::: {.callout-note icon=false}

## Example: Secchi

text
:::

::: {.callout-note}
text
:::



| from 0 to $d_{L}$ | from $d_{L}$ to $d_{U}$ | from $d_{U}$ to $4 - d_{U}$ | from $4 - d_{U}$ to $4 - d_{L}$ | from $4 - d_{L}$ to 4 |
|------|------|------|------|------|
| Reject $H_{0}$, positive autocorrelation | Neither accept $H_{1}$ or reject $H_{0}$ | Do not reject $H_{0}$ | Neither accept $H_{1}$ or reject $H_{0}$ | Reject $H_{0}$, negative autocorrelation |

: Regions of rejection of the null hypothesis for the Durbin--Watson test {#tbl-DW}


```
git checkout gh-pages # not used
git rebase master # not used
quarto publish gh-pages # not used
```
