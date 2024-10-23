# Nome do arquivo LaTeX principal (sem a extensão)
TARGET = proposta

# Comandos
LATEX = pdflatex
BIBTEX = bibtex

# Regras para gerar o PDF
all: $(TARGET).pdf

$(TARGET).pdf: $(TARGET).tex
	$(LATEX) $(TARGET).tex
	$(LATEX) $(TARGET).tex  # Rodar duas vezes para garantir referências corretas

# Limpar arquivos temporários gerados pelo LaTeX
clean:
	rm -f *.aux *.log *.out *.toc *.bbl *.blg

# Limpar tudo, incluindo o PDF gerado
cleanall: clean
	rm -f $(TARGET).pdf
