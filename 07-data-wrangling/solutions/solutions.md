# Invoice dates

## Per year report

```python
df.groupby(['InvoiceDate_Yr']).size()
```

or to calculate total sales

```python
df ['TotalSales'] = df['Quantity'] * df['UnitPrice']
df.sample(5)

df[['InvoiceDate_Yr', 'TotalSales']].groupby(['InvoiceDate_Yr']).sum()
```
