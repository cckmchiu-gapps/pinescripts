# PineScript Indicators

A collection of standalone TradingView Pine Script indicators and chart
utilities. Scripts are kept as `.txt` files so they can be copied into the
TradingView Pine Editor.

## Grid and chart-range tools

| File | Pine version | Overview |
| --- | --- | --- |
| [`GridWB3.txt`](./GridWB3.txt) | v5 | Manually set two opposite time-and-price anchors. Draws a price/time grid with quarter divisions and diagonals. |
| [`GridWB4.txt`](./GridWB4.txt) | v5 | Manually set two opposite anchors to draw a configurable grid, with a fine-tunable future right edge. |
| [`GridWB3_v5.txt`](./GridWB3_v5.txt) | v6 | Calculates price bounds from historical closing prices over a selected date range; includes grid-count, styling, and information-table options. |
| [`GridWB3_v6.txt`](./GridWB3_v6.txt) | v6 | Extends the automatic date-range version to account for symbols whose available history starts after the selected start date. |
| [`GridWB3_v7.txt`](./GridWB3_v7.txt) | v6 | Scales to the visible chart or a fixed date range, using the range's high and low prices. |
| [`四邊圖v10.txt`](./四邊圖v10.txt) | v6 | Advanced four-edge grid (V10.12) with independently draggable boundaries, configurable connected cells, horizontal alignment modes, and optional settlement-date alignment. |

The GridWB3/GridWB4 scripts draw rectangular price-and-time grids with
horizontal and vertical divisions and diagonal lines. Choose `GridWB3.txt` or
`GridWB4.txt` for manually positioned anchors; choose `GridWB3_v7.txt` for
visible-screen or fixed-date automatic scaling. The V10 four-edge tool provides
more independent boundary controls and alignment options.

## Other chart utilities

| File | Pine version | Overview |
| --- | --- | --- |
| [`CM_TotalConsecutive_Up_Down_V2.txt`](./CM_TotalConsecutive_Up_Down_V2.txt) | Legacy syntax | Plots consecutive up/down bar counts based on midpoint or previous close, with optional lookback highs, standard deviation, and moving-average plots. |
| [`MyNotes.txt`](./MyNotes.txt) | v5 | Displays selectable trading notes on the chart, with position, size, alignment, and color settings. |
| [`MyWatermark.txt`](./MyWatermark.txt) | v4 | Displays customizable text as a chart watermark. |

## Stock list

[`紅色清單.txt`](./紅色清單.txt) is a comma-separated list of Hong Kong-listed
tickers in `HKEX:<ticker>` format, organized under Chinese headings for leading
stocks, holdings, and watchlist stocks.

## Use with TradingView

1. Open the desired `.txt` file and copy its contents.
2. In TradingView, open the **Pine Editor** and paste the script.
3. Save the script and select **Add to chart**.
4. Configure the indicator using its settings and, where applicable, chart
   handles.

This repository has no build system or dependency manifest. Pine Script
compilation and chart behavior are checked in TradingView.
