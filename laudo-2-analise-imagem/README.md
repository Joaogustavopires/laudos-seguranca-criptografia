# 📸 Laudo Pericial 2: Análise Forense em Imagem Digital (placaMoto.jpeg)

## 🎯 Objetivo da Perícia
[cite_start]O trabalho pericial teve como objetivo a **análise forense do arquivo digital** `placaMoto.jpeg` [cite: 12][cite_start], visando responder aos quesitos apresentados pela parte Autora, com foco na integridade, tempo de captura, extração de informações visuais (placa) e estimativa de altura do condutor[cite: 12, 19].

---

## 🔬 Metodologia e Evidências Técnicas

[cite_start]O trabalho pericial seguiu as diretrizes do DFIR (Digital Forensics and Incident Response) e a Norma **ABNT ISO/IEC 27037:2013**, que estabelece padrões para a preservação da cadeia de custódia[cite: 10, 21].

### Preservação e Verificação de Integridade
* [cite_start]**Objeto:** O material examinado é o arquivo de imagem digital em formato JPEG, denominado `placaMoto.jpeg`[cite: 15].
* [cite_start]**HASHs de Integridade:** A integridade do arquivo é comprovada pelas HASHs calculadas com o **HashCalc**[cite: 16].
    * [cite_start]**MD5:** `d4233db838cf71eab9e1127a22e21803`[cite: 32].
    * [cite_start]**SHA-256:** `422f9d56432f14f0d07e26b6df625447b41e6a9b77311cb8324e8e3c5913f8f9`[cite: 34].
![Captura de tela do HashCalc com as HASHs](imagens/HASHCALC.png)
### Análise de Metadados e Temporal
* [cite_start]**Extração de Metadados:** Utilização do **ExifTool** para obtenção de dados estruturais[cite: 22].
* [cite_start]**Timestamp Original:** O campo `DateTimeOriginal` estava **ausente**[cite: 40, 46]. [cite_start]A data mais confiável é o timestamp embutido na imagem, indicando a captura às **10:40:39 de 12-01-2017**[cite: 40].
![Captura de tela do ExifTool e metadados](imagens/Exiftool.png)
### Análise de Adulteração (ELA)
* [cite_start]**Verificação da Integridade:** Utilização da ferramenta **Forensically** e análise **ELA** (Error Level Analysis)[cite: 23].
* **Conclusão Técnica:** Não foram encontrados sinais técnicos de adulteração. [cite_start]A análise ELA revelou um **padrão de compressão uniforme**, confirmando que o arquivo é um *snapshot* de vídeo sem manipulação posterior[cite: 44].
![Resultado da análise ELA pelo Forensically](imagens/Forensecally_ELA.png)
---

## ⚖️ Conclusão Pericial: Resultados e Respostas aos Quesitos

### Resultados da Análise de Conteúdo

* [cite_start]**Quesito 9 (Placa):** **NÃO foi possível identificar a placa da motocicleta de forma conclusiva**[cite: 50, 61]. [cite_start]A resolução e o nível de ruído não permitiram a legibilidade inequívoca dos caracteres após o processamento de imagem[cite: 51].
* **Quesito 11 (Altura):** **SIM**, foi possível estimar a altura do condutor.
    * [cite_start]**Processamento e Medição:** Utilizando o **ImageJ/Fiji** e calibração de escala[cite: 24, 55].
    * [cite_start]**Altura Estimada:** A altura estimada do condutor é de **1,87 metros** (Valor exato: 1,865 m)[cite: 55, 60].
![Captura de tela da medição no ImageJ/Fiji](imagens/MENSURE.png)
### Conclusão Final
[cite_start]A perícia permitiu estimar a altura do condutor em **1,87 m** [cite: 60] [cite_start]e confirmou que a imagem é um *snapshot* de sistema de vigilância (DVR)[cite: 59]. [cite_start]Contudo, não foi possível identificar a placa da motocicleta (Quesito 9) devido à baixa qualidade da imagem[cite: 61].
