Track statistics:



Test google every 2 seconds for 24 hours. Write results to test-google.csv:

./ping-csv.sh --add-timestamp -c 43200 -i 2 www.google.de > test-google.csv

Create plot from csv file:

gnuplot -c plot-stats.gp test-google.csv
