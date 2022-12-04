Todo
- check presence of comments "<!--" in QMD files to fix that.
- check that all labels # are cited (figures, tables)
- check grammar
- check :: and library() calls and add packages to the software list
- add an empty line between :| and code or comments in each chunk

# Format

Replace  
\boldsymbol with \bm  
Figure~\ref{fig: with @fig-

a.k.a.
changepoint
nonlinear
nonparametric
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

```
git checkout gh-pages # not used
git rebase master # not used
quarto publish gh-pages # not used
```
