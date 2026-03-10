# 📚 Web Scraping com Python

> Módulo 5 — Python Avançado | Curso Backend Python · EBAC

---

## 📋 Sobre o projeto

Exercício do **Módulo 5** do curso de Backend Python da EBAC.  
O projeto consiste em um scraper desenvolvido em Python que coleta dados de livros do site [books.toscrape.com](https://books.toscrape.com) — um site criado especificamente para praticar web scraping.

Os dados coletados (título, preço, disponibilidade e rating) são salvos em um arquivo `.csv`.

---

## 🚀 Funcionalidades

- ✅ Scraping de uma única página
- ✅ Scraping com paginação (múltiplas páginas)
- ✅ Scraping paralelizado com **threads**
- ✅ Exportação dos dados para `.csv`
- ✅ Comparação de desempenho: sequencial vs threads

---

## 🛠️ Tecnologias utilizadas

| Biblioteca | Uso |
|---|---|
| `requests` | Requisições HTTP |
| `beautifulsoup4` | Parsing do HTML |
| `concurrent.futures` | Paralelismo com threads |
| `threading` | Lock para escrita segura no CSV |
| `csv` | Exportação dos dados |

---

## ⚙️ Como executar

**1. Clone o repositório**
```bash
git clone https://github.com/SEU_USUARIO/python-scraping.git
cd python-scraping
```

**2. Instale as dependências**
```bash
pip install requests beautifulsoup4
```

**3. Execute o script**
```bash
python exercicio_scraping.py
```

Ou no **Jupyter / Google Colab**, chame cada parte separadamente:

```python
parte1()              # Scraping de 1 página
parte2()              # Scraping com paginação
parte3()              # Scraping com threads
parte3_comparacao()   # Comparação de desempenho
```

---

## 📁 Estrutura do projeto

```
python-scraping/
│
├── exercicio_scraping.py   # Script principal
├── livros_parte2.csv       # Resultado da Parte 2 (gerado ao executar)
├── livros_parte3.csv       # Resultado da Parte 3 (gerado ao executar)
└── README.md
```

---

## 🧠 Conceitos praticados

- Requisições HTTP com `requests`
- Parsing de HTML com `BeautifulSoup`
- Navegação por paginação
- Paralelismo com `ThreadPoolExecutor`
- Controle de concorrência com `threading.Lock`
- Exportação de dados para CSV

---

## 📖 Exemplo de saída

```
==================================================
PARTE 1 — Scraping de 1 página
==================================================
Livros encontrados: 20

  📚 A Light in the Attic
     Preço: £51.77 | Rating: Three | In stock

  📚 Tipping the Velvet
     Preço: £53.74 | Rating: One | In stock
```

---

<div align="center">
  Feito durante o curso <strong>Backend Python</strong> · <a href="https://ebaconline.com.br">EBAC</a>
</div>
