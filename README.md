# gee-landcover-foz-do-iguacu

# Mapeamento de Uso do Solo em Foz do Iguaçu (2021) com GEE

Este projeto utiliza o Google Earth Engine (GEE), imagens Sentinel-2 e um classificador de Machine Learning (Random Forest) para criar um mapa de cobertura do solo de alta resolução para o município de Foz do Iguaçu.

---

## Objetivo
O objetivo foi classificar o município em 4 classes principais para entender a distribuição da paisagem em 2021:
* Área Urbana
* Água
* Floresta
* Agricultura/Pasto

## Metodologia
O fluxo de trabalho seguiu os passos profissionais para análise de sensoriamento remoto:
1.  **Coleta de Dados:** Imagens Sentinel-2 (SR) para todo o ano de 2021.
2.  **Limpeza (Pré-processamento):** Criação de um mosaico limpo e sem nuvens usando o algoritmo Google Cloud Score+ (`cs_cdf`).
3.  **Treinamento:** Coleta de amostras de treinamento para as 4 classes.
4.  **Classificação (Machine Learning):** Treinamento de um classificador `smileRandomForest` com 50 árvores.
5.  **Resultado:** Geração de um mapa de classificação final de 10m de resolução.


LinkCode:https://code.earthengine.google.com/3c9c54bd7ef40673e167594979d48a05
