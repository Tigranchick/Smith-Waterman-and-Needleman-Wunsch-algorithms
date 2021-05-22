# Smith-Waterman-and-Needleman-Wunsch-algorithms
The main purpose is just visualize the matrices produced due to the alignment of proteins. There are adjunction of use blosum62 and PAM250 score matrices.
 
The example result in "Smith-Waterman-matrix-and-alignment.py"

SmithWaterman( 'QESGLVRC','QKESGPSYC', PAM_250)

score matrix = 
[[  0.  -2.  -4.  -6.  -8. -10. -12. -14. -16. -18.]
 [ -2.   4.   2.   0.  -2.  -4.  -6.  -8. -10. -12.]
 [ -4.   2.   4.   6.   4.   2.   0.  -2.  -4.  -6.]
 [ -6.   0.   2.   4.   8.   6.   4.   2.   0.  -2.]
 [ -8.  -2.   0.   2.   6.  13.  11.   9.   7.   5.]
 [-10.  -4.  -2.   0.   4.  11.  10.   8.   8.   6.]
 [-12.  -6.  -4.  -2.   2.   9.  10.   9.   7.   6.]
 [-14.  -8.  -3.  -4.   0.   7.   9.  10.   8.   6.]
 [-16. -10.  -5.  -6.  -2.   5.   7.   9.  10.  20.]]

[calculation process of traceback]

Identity = 50.0 percent
Score = 20n
Q-ESGLVR-C
Q ESG    C
QKESG-PSYC

 
The example result in "Needleman-Wunsch-matrix.py"

NeedlemanWunsch('QESGLVRC','QKESGPSYC', PAM_250)

score matrix = 
[[ 0.  0.  0.  0.  0.  0.  0.  0.  0.  0.]
 [ 0.  4.  2.  2.  0.  0.  0.  0.  0.  0.]
 [ 0.  2.  4.  6.  4.  2.  0.  0.  0.  0.]
 [ 0.  0.  2.  4.  8.  6.  4.  2.  0.  0.]
 [ 0.  0.  0.  2.  6. 13. 11.  9.  7.  5.]
 [ 0.  0.  0.  0.  4. 11. 10.  8.  8.  6.]
 [ 0.  0.  0.  0.  2.  9. 10.  9.  7.  6.]
 [ 0.  1.  3.  1.  0.  7.  9. 10.  8.  6.]
 [ 0.  0.  1.  0.  1.  5.  7.  9. 10. 20.]]

