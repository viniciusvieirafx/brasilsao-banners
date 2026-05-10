# Brasilsão — Banners

Repositório de imagens dos banners rotativos do mundo VRChat **Brasilsão**.

---

## Como funciona

O mundo baixa **uma única imagem** (`banner_grid.png`) que contém todos os banners organizados em uma grade 4×N.  
O shader `BannerSystem/BannerScroll` desliza entre os painéis automaticamente.

**Não edite os arquivos diretamente aqui.** Use o script de upload.

---

## Adicionar / trocar banners

1. Coloque as imagens novas na pasta `Upload/` (dentro de `Send Banners/`)
2. Rode `Upar Imagens.bat` (duplo clique)
3. Pronto — o mundo atualiza automaticamente na próxima vez que alguém entrar

**Requisito:** `pip install Pillow` (só na primeira vez)

---

## Especificações das imagens

| Parâmetro | Valor |
|---|---|
| Resolução recomendada | 1920×1080 (16:9) |
| Resolução máxima | 2048×2048 |
| Formatos aceitos | PNG, JPG, JPEG, WEBP |
| Tamanho máximo | 5 MB por arquivo |

---

## URL da grade (Unity Inspector)

```
https://raw.githubusercontent.com/viniciusvieirafx/brasilsao-banners/main/banner_grid.png
```

Cole essa URL no campo **Grid Image Url** do componente `BannerManager` na cena.  
Não muda — mesmo quando os banners são atualizados.

---

## Capacidade

Grade fixa de **4 colunas × célula 512×288 px** dentro de 2048×2048:

| Banners | Grade | Tamanho da imagem |
|---|---|---|
| 1–4 | 4×1 | 2048×288 |
| 5–8 | 4×2 | 2048×576 |
| 9–12 | 4×3 | 2048×864 |
| 13–16 | 4×4 | 2048×1152 |
| 17–20 | 4×5 | 2048×1440 |
| 21–24 | 4×6 | 2048×1728 |
| 25–28 | 4×7 | 2048×2016 |
