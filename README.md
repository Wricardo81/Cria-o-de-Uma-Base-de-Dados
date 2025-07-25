# 🔍 Detecção de Objetos com YOLOv5 — Caneca e Celular

Este projeto implementa um modelo de **detecção de objetos personalizado** utilizando **YOLOv5** com **Transfer Learning** no Google Colab. As classes detectadas são:

- 📱 `celular`
- ☕ `caneca`

## 📁 Estrutura do Projeto

custom_dataset/
├── images/
│ ├── caneca.jpg
│ ├── celular.jpg
├── labels/
│ ├── caneca.txt
│ ├── celular.txt

yaml
Copiar
Editar


## 🛠️ Tecnologias

- [YOLOv5](https://github.com/ultralytics/yolov5)
- Google Colab
- Python 3
- LabelMe (para anotação de imagens)

---

## 🚀 Etapas do Projeto

### 1. Anotação dos Dados

As imagens foram rotuladas com o [LabelMe](http://labelme.csail.mit.edu/Release3.0/) e convertidas para o formato YOLO.

### 2. Upload no Google Colab

Faça upload do `.zip` contendo a pasta `custom_dataset/` com subpastas `images/` e `labels/`.

### 3. Treinamento com Transfer Learning

O modelo YOLOv5 foi treinado usando pesos pré-treinados (`yolov5s.pt`) e duas novas classes.

### 4. Avaliação e Inferência

Após o treinamento, é possível visualizar os gráficos de desempenho e testar o modelo em novas imagens.

---

## 📓 Notebook

Você pode acessar o notebook completo [aqui](https://colab.research.google.com/) ou abrir localmente este arquivo:

- `YOLOv5_Transfer_Learning_Caneca_Celular.ipynb`

---

## 📦 Requisitos

Caso deseje rodar localmente:

```bash
git clone https://github.com/ultralytics/yolov5
cd yolov5
pip install -r requirements.txt
