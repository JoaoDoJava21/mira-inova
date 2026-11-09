# MIRA no INOVA NACIONAL 2026

Site do estande do MIRA (Modelo de Inspeção e Resposta Autônoma): um chat no estilo mensageiro em que a IA confere capacete e colete por foto e libera a entrada na obra, uma demonstração animada e um manual de EPI.

A detecção roda no navegador do visitante, com o modelo `mira_ppe` (YOLO26n exportado para ONNX) e o [onnxruntime-web](https://github.com/microsoft/onnxruntime) 1.20.1 em `ort/`. As fotos não saem do aparelho.

- `index.html`: o site inteiro (HTML, CSS e JS)
- `mira_ppe.onnx`: modelo de detecção (capacete, SEM capacete, colete, SEM colete, pessoa)
- `img/`: fotos reais com as caixas desenhadas pelo modelo; créditos no fim da página do manual

Fotos: Flickr, licença CC BY 2.0 (autores listados no manual). Modelo baseado no Ultralytics YOLO (AGPL-3.0), treinado com o dataset Construction Site Safety (Roboflow, CC BY 4.0).
