Conversor R
================
Ana Paula e Gabriel Gouveia
04/03/2021

## Instalacao

Baixe o pacote com:

``` r
install.packages("devtools")
install.packages("shiny")
devtools::install_github("GShotwell/convertr")
```

## Uso

O pacote contém uma função que converte vetores numéricos de uma unidade
para outra. Os dados sobre os fatores de conversão vêm do Dicionário de
Unidades de Medida POSC v2.2 e da Wikipedia.

As unidades são convertidas usando uma tabela de pesquisa, com base no
dicionário POSC. Você pode explorar esta tabela usando a função
explore\_units (). Esta função inicia um aplicativo brilhante.

Descobrir quais unidades podem ser convertidas entre si pode ser
complicado, então convertr vem com um gadget brilhante para ajudá-lo a
construir expressões convert () válidas. Isso pode ser acessado chamando
convert\_gadget () ou através do menu addin. Para acessar o addin,
certifique-se de estar usando uma versão recente do RStudio.

## Exemplo

Adicionar a biblioteca

``` r
library("convertr")
```

Ou usar apenas os comandos da biblioteca pela classe, como abaixo:

Conversão de Km/h para m/s:

``` r
convertr::convert(108,'km/h','m/s')
```

    ## [1] 30

Conversão de pressão, Bar para Kpa:

``` r
convertr::convert(1,'bar','kPa')
```

    ## [1] 100

# Modo Gráfico

![Primeiro Passo](exemplo%201.png) ![Segundo Passo](exemplo%202.png)

## Creditos

``` r
https://github.com/cran/convertr
```
