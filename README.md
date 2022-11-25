
# Format

**Objectives**

and 

**Reading materials**

in bold. Use *italics* for highlights in text.

Use 'single quotes' whenever possible.

Cite 
@Brockwell:Davis:2002
or 
[@Brockwell:Davis:2002]


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

\bm replace with \boldsymbol 
Figure~\ref{fig: replace with @fig-

# GitHub

Write in `master`, then update `gh-pages`.

::: {.callout-note icon=false}

## Example: Secchi

sds
:::



```
git checkout gh-pages
git rebase master
quarto publish gh-pages # not used
```
