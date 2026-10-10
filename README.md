# BuilderGS6
A modified builder for the offline game gridless sekai 6.
the official repo: https://github.com/UnknownSekai/GridlessSekai6
the forked repo for cmd window (the builder is based on it): https://github.com/733402/gs6

>What's implemented?
-Command for making chart even if they have mismatched combos
-prewiev music cutter
- .json/.json.gz files can be transformed into charts
- it allows layers to be added to the chart
# Commands for things

allow combo mismatch: --allow-combo-mismatch (example: python3 main.py yourconvertedchart.zip --allow-combo-mismatch)

prewiec music cutter: ffmpeg -ss 30 -t 30 -i preview.mp3 -af "afade=t=in:d=1,afade=t=out:st=29:d=1" preview_short.mp3 (open in the chart folder)

# How to make charts from .json/.json.gz files
in builder : python3 main.py yourchartfolder.zip
