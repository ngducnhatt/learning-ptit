1. BFS
STT | Nút được mở rộng | Tập biên O
-----------------------------------
0	|					| S
1	|S 					| Ds Es Ps
2	|Ds					| Es Ps Bd Cd
3 	|Es					| Ps Bd Cd He Re
4 	|Ps					| Bd Cd He Re Qp
5 	|Bd					| Cd He Re Qp Ab
6 	|Cd					| He Re Qp Ab
7 	|He					| Re Qp Ab
8 	|Re					| Qp Ab Fr
9 	|Qp					| Ab Fr
10 	|Ab					| Fr
11 	|Fr					| Gf
12 	|Gf					| Goal

G - F - R - E - S 

2. UCS
STT | Nút được mở rộng | Tập biên O
-----------------------------------
0	|					| S
1	|S 					| Ds(3) Es(9) Ps(1)
2	|Ps					| Ds(3) Es(9) Qp(2)
3	|Qp					| Ds(3) Es(9) Rq(5)
4 	|Ds					| Es(9) Rq(5) Bd(4) Cd(11) Ed(5)
5	|Bd					| Es(9) Rq(5) Cd(11) Ed(5) Ab(6)
5	|Ed					| Es(9) Rq(5) Cd(11) Ab(6) He(6) Re(14)
6	|Rq					| Es(9) Cd(11) Ab(6) He(6) Re(14) Fr(5)
7	|Fr					| Es(9) Cd(11) Ab(6) He(6) Re(14) Gf(15)
8	|Gf					| Goal

G - F - R - Q - P - S vs độ dài là 15

3.DFS
STT | Nút được mở rộng | Tập biên O
-----------------------------------
0	|					| S
1	|S 					| As Bs
2	|As					| Ca Bs
3 	|Ca					| Dc Ec Bs
4 	|Dc					| Fd Ec Bs
5 	|Fd					| Gf Ec Bs
6 	|Gf					| Goal

G - F - D - C - A - S

4.IDS
STT | Nút được mở rộng | Tập biên O
-----------------------------------
c = 0
0	|					| S
1	|S 					| rỗng
c = 1
0	|					| Sß
1 	|S					| As Bs
2 	|As					| Bs
3 	|Bs					| As
c = 2
0	|					| S
1 	|S					| As Bs
2 	|As					| Ca Bs
3	|Ca					| Dc Ec Bs
4	|Dc					| Fd Ec Bs
5	|Fd 				| Gf Ec Bs
6 	|Gf					| Goal

G - F - D - C - A - S vs độ sâu c = 2