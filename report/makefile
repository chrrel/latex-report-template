DOCUMENT_NAME = report
OUTPUT_DIR    = out

all: report

# Remove output directory.
clean:
	rm -rf $(OUTPUT_DIR)

# Generate PDF from LaTex files.
report:
	mkdir -p $(OUTPUT_DIR)
	latexmk -pdf -jobname=$(OUTPUT_DIR)/$(DOCUMENT_NAME) report.tex
	mv $(OUTPUT_DIR)/$(DOCUMENT_NAME).pdf $(DOCUMENT_NAME).pdf 
