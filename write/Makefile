#
# Authors:     PN
# Maintainers: PN
# Copyright:   2024, UWCHR, GPL v2 or later
# ============================================
# describe-sea/write/Makefile

.PHONY: all

all: \
	output/border-everywhere.html

clean:
	rm -r output/*

output/border-everywhere.html: \
		note/border-everywhere.Rmd \
		../import/input/ice_encounters_fy12-23ytd.csv.gz \
		../import/input/ice_arrests_fy12-23ytd.csv.gz \
		../import/input/ice_removals_fy12-23ytd.csv.gz \
		../import/input/ice_detentions_fy12-24ytd.csv.gz \
		../import/input/ice_unique_stays_fy12-24ytd.csv.gz \
		../import/input/headcount_fy12-24ytd.csv.gz \
		../import/input/uw-chr-i213-public.csv.gz \
		../import/input/usbp_monthly_encounters_fy2000-fy2020.csv.gz \
		../import/input/cbp-nationwide-encounters-fy20-fy23-aor.csv \
		../import/input/cbp-nationwide-encounters-fy20-fy23-state.csv
	mkdir -p input output
	cd input && ln -sf ../../import/input/* .
	Rscript -e "rmarkdown::render('note/border-everywhere.Rmd', 'html_document')"
	mv note/border-everywhere.html output/
	mv note/*.png output/

# done.
