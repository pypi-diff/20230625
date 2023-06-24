# Comparing `tmp/higlass_schema-0.0.6.tar.gz` & `tmp/higlass_schema-0.1.0.tar.gz`

## Comparing `higlass_schema-0.0.6.tar` & `higlass_schema-0.1.0.tar`

### file list

```diff
@@ -1,101 +1,102 @@
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/.github/dependabot.yml
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/higlass_schema/__init__.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/higlass_schema/cli.py
--rw-r--r--   0        0        0    16562 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/higlass_schema/schema.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/higlass_schema/utils.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/test_schema.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/README.md
--rw-r--r--   0        0        0    10226 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/1d-annotations.json
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/1d-constant-indicators.json
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/1d-heatmap-track-2.json
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/1d-heatmap-track.json
--rw-r--r--   0        0        0     8155 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/axis-margin.json
--rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/bar-track-color-range.json
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/bar-track.json
--rw-r--r--   0        0        0     5870 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/bar-zero-line.json
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/bedlike-track.json
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/bigwig-aggregation-modes.json
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/chromosome-labels.json
--rw-r--r--   0        0        0    10769 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/default.json
--rw-r--r--   0        0        0     8275 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/diagonal-split-heatmap.json
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/fancy-overlays.json
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/genbank-data-fetcher.json
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/gene-annotations.json
--rw-r--r--   0        0        0     7519 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/label-margin.json
--rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/lots-of-locks.json
--rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/overlay-chromosome-grid-track.json
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/overlay-track.json
--rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/overlay-tracks.json
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/adjust-view-spacing.json
--rw-r--r--   0        0        0     8103 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/axis-specific-location-locks.json
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/axis.json
--rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/bar.json
--rw-r--r--   0        0        0    10636 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/continuous-scaling-1D-horizontal.json
--rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/continuous-scaling-1D-vertical.json
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/continuous-scaling-2D.json
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/dummy-data-fetcher.json
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/dummy-track.json
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/global-mouse-position.json
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/horizontal-1d-line-track-with-const.json
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/label-margin.json
--rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/label-split-heatmaps.json
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/loop-annotations.json
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/overlay-annotations-1d-2d.json
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/overlay-chrom-grid.json
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/simple-1d-horizontal-vertical-and-2d-data-track.json
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/simple-heatmap-gene-annotations.json
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/simple-heatmap.json
--rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/two-bars-and-a-heatmap.json
--rw-r--r--   0        0        0     8154 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs/viewport-projection.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-invalid/invalidTrackConfig.json
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/annotationsTilesView.json
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/divergentTrackConfig.json
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/divisionViewConfig.json
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/emptyConf.json
--rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/exportDataConfig.json
--rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/fritzBug1.json
--rw-r--r--   0        0        0   100356 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/fritzBug2.json
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/geneAnnotationsOnly.json
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/geneAnnotationsOnly1.json
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/horizontalAndVerticalMultivec.json
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/horizontalDiagonalTrackViewConf.json
--rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/horizontalLineEnd.json
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/horizontalMultivecWithAggregation.json
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/horizontalMultivecWithFilteredRows.json
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/horizontalMultivecWithSmallerDimensions.json
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/horizontalMultivecWithZeroValueColorOption.json
--rw-r--r--   0        0        0    21964 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/local-tiles-viewconf.json
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/noGPSB.json
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/oneTrackConfig.json
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/oneViewConfig.json
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/oneZoomedOutViewConf.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/onlyGPSB.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/osmConf.json
--rw-r--r--   0        0        0    17615 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/paperFigure1.json
--rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/project1D.json
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/rectangleDomains.json
--rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/restrictedZoom.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/simple1And2dAnnotations.json
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/simpleCenterViewConfig.json
--rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/smallViewconf.json
--rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/stacked-top-tracks.json
--rw-r--r--   0        0        0    31108 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/stacked-top-views.json
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/testViewConfX1.json
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/testViewConfX2.json
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/threeViews.json
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/topAxisOnly.json
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/twoViewConfig.json
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/valueIntervalTrackViewConf.json
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/viewportProjectionsWithoutFromViewUids.json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-tracks/chromInfoTrack.json
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-tracks/chromosomeGridTrack.json
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-tracks/heatmapTrack.json
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-tracks/horizontalHeatmapTrack.json
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-tracks/largeHorizontalHeatmapTrack.json
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/tests/fixtures/test/view-configs-tracks/verticalHeatmapTrack.json
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/LICENSE
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/README.md
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 higlass_schema-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/higlass_schema/__init__.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/higlass_schema/cli.py
+-rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/higlass_schema/schema.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/higlass_schema/utils.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/test_schema.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/README.md
+-rw-r--r--   0        0        0    10226 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/1d-annotations.json
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/1d-constant-indicators.json
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/1d-heatmap-track-2.json
+-rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/1d-heatmap-track.json
+-rw-r--r--   0        0        0     8155 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/axis-margin.json
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/bar-track-color-range.json
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/bar-track.json
+-rw-r--r--   0        0        0     5870 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/bar-zero-line.json
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/bedlike-track.json
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/bigwig-aggregation-modes.json
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/chromosome-labels.json
+-rw-r--r--   0        0        0    10769 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/default.json
+-rw-r--r--   0        0        0     8275 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/diagonal-split-heatmap.json
+-rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/fancy-overlays.json
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/genbank-data-fetcher.json
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/gene-annotations.json
+-rw-r--r--   0        0        0     7519 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/label-margin.json
+-rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/lots-of-locks.json
+-rw-r--r--   0        0        0     3620 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/overlay-chromosome-grid-track.json
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/overlay-track.json
+-rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/overlay-tracks.json
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/adjust-view-spacing.json
+-rw-r--r--   0        0        0     8103 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/axis-specific-location-locks.json
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/axis.json
+-rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/bar.json
+-rw-r--r--   0        0        0    10636 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/continuous-scaling-1D-horizontal.json
+-rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/continuous-scaling-1D-vertical.json
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/continuous-scaling-2D.json
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/dummy-data-fetcher.json
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/dummy-track.json
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/global-mouse-position.json
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/horizontal-1d-line-track-with-const.json
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/label-margin.json
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/label-split-heatmaps.json
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/loop-annotations.json
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/overlay-annotations-1d-2d.json
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/overlay-chrom-grid.json
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/simple-1d-horizontal-vertical-and-2d-data-track.json
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/simple-heatmap-gene-annotations.json
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/simple-heatmap.json
+-rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/two-bars-and-a-heatmap.json
+-rw-r--r--   0        0        0     8154 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs/viewport-projection.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-invalid/invalidTrackConfig.json
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/annotationsTilesView.json
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/divergentTrackConfig.json
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/divisionViewConfig.json
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/emptyConf.json
+-rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/exportDataConfig.json
+-rw-r--r--   0        0        0    50011 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/fritzBug1.json
+-rw-r--r--   0        0        0   100356 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/fritzBug2.json
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/geneAnnotationsOnly.json
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/geneAnnotationsOnly1.json
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/horizontalAndVerticalMultivec.json
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/horizontalDiagonalTrackViewConf.json
+-rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/horizontalLineEnd.json
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/horizontalMultivecWithAggregation.json
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/horizontalMultivecWithFilteredRows.json
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/horizontalMultivecWithSmallerDimensions.json
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/horizontalMultivecWithZeroValueColorOption.json
+-rw-r--r--   0        0        0    21964 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/local-tiles-viewconf.json
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/noGPSB.json
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/oneTrackConfig.json
+-rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/oneViewConfig.json
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/oneZoomedOutViewConf.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/onlyGPSB.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/osmConf.json
+-rw-r--r--   0        0        0    17615 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/paperFigure1.json
+-rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/project1D.json
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/rectangleDomains.json
+-rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/restrictedZoom.json
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/simple1And2dAnnotations.json
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/simpleCenterViewConfig.json
+-rw-r--r--   0        0        0     5962 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/smallViewconf.json
+-rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/stacked-top-tracks.json
+-rw-r--r--   0        0        0    31108 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/stacked-top-views.json
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/testViewConfX1.json
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/testViewConfX2.json
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/threeViews.json
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/topAxisOnly.json
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/twoViewConfig.json
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/valueIntervalTrackViewConf.json
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/viewportProjectionsWithoutFromViewUids.json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-tracks/chromInfoTrack.json
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-tracks/chromosomeGridTrack.json
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-tracks/heatmapTrack.json
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-tracks/horizontalHeatmapTrack.json
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-tracks/largeHorizontalHeatmapTrack.json
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/tests/fixtures/test/view-configs-tracks/verticalHeatmapTrack.json
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/LICENSE
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/README.md
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 higlass_schema-0.1.0/PKG-INFO
```

### Comparing `higlass_schema-0.0.6/.github/workflows/ci.yml` & `higlass_schema-0.1.0/.github/workflows/ci.yml`

 * *Files 27% similar despite different names*

```diff
@@ -42,47 +42,21 @@
       - run: ajv validate -s schema.json -d "tests/fixtures/{docs/examples/viewconfs,test/{view-configs,view-configs-more}}/*.json"
 
   Test:
     name: Test ${{ matrix.python-version }}
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.8', '3.9', '3.10', '3.11']
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           pipx install hatch
           hatch run test
-
-  Release:
-    # this will run when you have tagged a commit, starting with "v*"
-    # and requires that you have put your twine API key in your 
-    # github secrets (see readme for details)
-    needs: [Test]
-    runs-on: ubuntu-latest
-    if: contains(github.ref, 'tags')
-    steps:
-      - uses: actions/checkout@v3
-      - name: Set up Python
-        uses: actions/setup-python@v4
-        with:
-          python-version: "3.x"
-      - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          pip install build twine
-      - name: Build and publish
-        env:
-          TWINE_USERNAME: __token__
-          TWINE_PASSWORD: ${{ secrets.TWINE_API_KEY }}
-        run: |
-          git tag
-          python -m build .
-          twine upload dist/*
```

### Comparing `higlass_schema-0.0.6/higlass_schema/cli.py` & `higlass_schema-0.1.0/higlass_schema/cli.py`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/higlass_schema/schema.py` & `higlass_schema-0.1.0/higlass_schema/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,32 +224,34 @@
 
 class AxisSpecificLocks(BaseModel):
     x: Optional[AxisSpecificLock] = None
     y: Optional[AxisSpecificLock] = None
 
 
 class LocationLocks(BaseModel):
-    locksByViewUid: Dict[str, Union[str, AxisSpecificLocks]] = {}
-    locksDict: Dict[str, Lock] = {}
+    locksByViewUid: Dict[str, Union[str, AxisSpecificLocks]] = Field(
+        default_factory=dict
+    )
+    locksDict: Dict[str, Lock] = Field(default_factory=dict)
 
 
 class ZoomLocks(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    locksByViewUid: Dict[str, str] = {}
-    locksDict: Dict[str, Lock] = {}
+    locksByViewUid: Dict[str, str] = Field(default_factory=dict)
+    locksDict: Dict[str, Lock] = Field(default_factory=dict)
 
 
 class ValueScaleLocks(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    locksByViewUid: Dict[str, str] = {}
-    locksDict: Dict[str, ValueScaleLock] = {}
+    locksByViewUid: Dict[str, str] = Field(default_factory=dict)
+    locksDict: Dict[str, ValueScaleLock] = Field(default_factory=dict)
 
 
 ##################################################
 # Tracks                                         #
 ##################################################
 
 TrackTypeT = TypeVar("TrackTypeT", bound=str)
```

### Comparing `higlass_schema-0.0.6/higlass_schema/utils.py` & `higlass_schema-0.1.0/higlass_schema/utils.py`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/test_schema.py` & `higlass_schema-0.1.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/1d-annotations.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/1d-annotations.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/1d-constant-indicators.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/1d-constant-indicators.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/1d-heatmap-track-2.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/1d-heatmap-track-2.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/1d-heatmap-track.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/1d-heatmap-track.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/axis-margin.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/axis-margin.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/bar-track-color-range.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/bar-track-color-range.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/bar-track.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/bar-track.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/bar-zero-line.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/bar-zero-line.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/bedlike-track.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/bedlike-track.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/bigwig-aggregation-modes.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/bigwig-aggregation-modes.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/chromosome-labels.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/chromosome-labels.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/default.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/default.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/diagonal-split-heatmap.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/diagonal-split-heatmap.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/fancy-overlays.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/fancy-overlays.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/genbank-data-fetcher.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/genbank-data-fetcher.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/gene-annotations.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/gene-annotations.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/label-margin.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/label-margin.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/lots-of-locks.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/lots-of-locks.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/overlay-chromosome-grid-track.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/overlay-chromosome-grid-track.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/overlay-track.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/overlay-track.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/docs/examples/viewconfs/overlay-tracks.json` & `higlass_schema-0.1.0/tests/fixtures/docs/examples/viewconfs/overlay-tracks.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/adjust-view-spacing.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/adjust-view-spacing.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/axis-specific-location-locks.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/axis-specific-location-locks.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/axis.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/axis.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/bar.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/bar.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/continuous-scaling-1D-horizontal.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/continuous-scaling-1D-horizontal.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/continuous-scaling-1D-vertical.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/continuous-scaling-1D-vertical.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/continuous-scaling-2D.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/continuous-scaling-2D.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/dummy-data-fetcher.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/dummy-data-fetcher.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/dummy-track.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/dummy-track.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/global-mouse-position.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/global-mouse-position.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/horizontal-1d-line-track-with-const.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/horizontal-1d-line-track-with-const.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/label-margin.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/label-margin.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/label-split-heatmaps.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/label-split-heatmaps.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/loop-annotations.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/loop-annotations.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/overlay-annotations-1d-2d.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/overlay-annotations-1d-2d.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/overlay-chrom-grid.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/overlay-chrom-grid.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/simple-1d-horizontal-vertical-and-2d-data-track.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/simple-1d-horizontal-vertical-and-2d-data-track.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/simple-heatmap-gene-annotations.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/simple-heatmap-gene-annotations.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/simple-heatmap.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/simple-heatmap.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/two-bars-and-a-heatmap.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/two-bars-and-a-heatmap.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs/viewport-projection.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs/viewport-projection.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-invalid/invalidTrackConfig.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-invalid/invalidTrackConfig.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/annotationsTilesView.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/annotationsTilesView.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/divergentTrackConfig.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/divergentTrackConfig.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/divisionViewConfig.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/divisionViewConfig.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/exportDataConfig.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/exportDataConfig.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/fritzBug1.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/fritzBug1.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/fritzBug2.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/fritzBug2.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/geneAnnotationsOnly.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/geneAnnotationsOnly.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/geneAnnotationsOnly1.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/geneAnnotationsOnly1.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/horizontalAndVerticalMultivec.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/horizontalAndVerticalMultivec.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/horizontalDiagonalTrackViewConf.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/horizontalDiagonalTrackViewConf.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/horizontalLineEnd.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/horizontalLineEnd.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/horizontalMultivecWithAggregation.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/horizontalMultivecWithAggregation.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/horizontalMultivecWithFilteredRows.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/horizontalMultivecWithFilteredRows.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/horizontalMultivecWithSmallerDimensions.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/horizontalMultivecWithSmallerDimensions.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/horizontalMultivecWithZeroValueColorOption.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/horizontalMultivecWithZeroValueColorOption.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/local-tiles-viewconf.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/local-tiles-viewconf.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/noGPSB.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/noGPSB.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/oneTrackConfig.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/oneTrackConfig.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/oneViewConfig.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/oneViewConfig.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/oneZoomedOutViewConf.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/oneZoomedOutViewConf.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/onlyGPSB.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/onlyGPSB.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/osmConf.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/osmConf.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/paperFigure1.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/paperFigure1.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/project1D.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/project1D.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/rectangleDomains.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/rectangleDomains.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/restrictedZoom.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/restrictedZoom.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/simple1And2dAnnotations.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/simple1And2dAnnotations.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/simpleCenterViewConfig.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/simpleCenterViewConfig.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/smallViewconf.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/smallViewconf.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/stacked-top-tracks.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/stacked-top-tracks.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/stacked-top-views.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/stacked-top-views.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/testViewConfX1.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/testViewConfX1.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/testViewConfX2.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/testViewConfX2.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/threeViews.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/threeViews.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/topAxisOnly.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/topAxisOnly.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/twoViewConfig.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/twoViewConfig.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/valueIntervalTrackViewConf.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/valueIntervalTrackViewConf.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-more/viewportProjectionsWithoutFromViewUids.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-more/viewportProjectionsWithoutFromViewUids.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-tracks/heatmapTrack.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-tracks/heatmapTrack.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-tracks/horizontalHeatmapTrack.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-tracks/horizontalHeatmapTrack.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-tracks/largeHorizontalHeatmapTrack.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-tracks/largeHorizontalHeatmapTrack.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/tests/fixtures/test/view-configs-tracks/verticalHeatmapTrack.json` & `higlass_schema-0.1.0/tests/fixtures/test/view-configs-tracks/verticalHeatmapTrack.json`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/LICENSE` & `higlass_schema-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/README.md` & `higlass_schema-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `higlass_schema-0.0.6/pyproject.toml` & `higlass_schema-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -19,18 +19,17 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
 url = { homepage = "https://github.com/higlass/higlass-schema" }
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dynamic = ["version"]
 dependencies = [
-    "importlib_metadata ; python_version < '3.8'",
     "pydantic>=1.10,<2.0",
     "rich>=13.3.3",
 ]
 
 [project.optional-dependencies]
 dev = [
   "black",
@@ -47,22 +46,29 @@
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.envs.default]
 features = ["dev"]
 
 [tool.hatch.envs.default.scripts]
-fix = "black . && ruff --fix ."
-lint = "black --check . && ruff ."
+lint = [
+  "ruff {args:.}",
+  "black --check --diff {args:.}",
+]
+fmt = [
+  "black {args:.}",
+  "ruff --fix {args:.}",
+  "lint",
+]
 test = "pytest ."
 
 # https://github.com/charliermarsh/ruff
 [tool.ruff]
 line-length = 88
-target-version = "py37"
+target-version = "py38"
 src = ["src", "tests"]
 extend-select = [
     "E",    # style errors
     "F",    # flakes
     "I",    # isort
     "UP",   # pyupgrade
     "RUF",  # ruff-specific rules
```

### Comparing `higlass_schema-0.0.6/PKG-INFO` & `higlass_schema-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: higlass-schema
-Version: 0.0.6
+Version: 0.1.0
 Summary: Pydantic models for HiGlass
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Requires-Dist: importlib-metadata; python_version < '3.8'
+Requires-Python: >=3.8
 Requires-Dist: pydantic<2.0,>=1.10
 Requires-Dist: rich>=13.3.3
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Description-Content-Type: text/markdown
```

