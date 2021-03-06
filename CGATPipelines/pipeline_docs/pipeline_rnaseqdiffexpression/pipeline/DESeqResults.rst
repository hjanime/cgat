=============
DESeq Results
=============

Differential expression
=============================

Summary
-------

The following table summarizes the results of the test for differential expression.
It lists for every combination of object (gene, isoform, ...), geneset and pair of tracks
the number of tests that passed, failed, etc.

+----------------------------------------+----------------------------------------+
|*Column*                                |*Content*                               |
+----------------------------------------+----------------------------------------+
|significant                             |Number of significant tests             |
+----------------------------------------+----------------------------------------+
|tested                                  |Number of tests in total                |
+----------------------------------------+----------------------------------------+
|status_OK                               |Number of successful tests              |
+----------------------------------------+----------------------------------------+
|twofold                                 |Number of significant tests, where the  |
|                                        |expression level differs by at least a  |
|                                        |factor of 2.                            |
+----------------------------------------+----------------------------------------+

.. report:: DifferentialExpression.TrackerDESummaryDESeq
   :render: table

   Table of DESeq differential expression results

.. report:: DifferentialExpression.TrackerDESummaryDESeq
   :render: interleaved-bar-plot
   :force:
   :slices: significant

   Number of significant tests

Diagnostic plots
----------------

.. report:: Tracker.TrackerImages 
   :render: gallery-plot    
   :tracker: deseq.dir/*.png
   
   Diagnostic plots from the DESeq analysis
