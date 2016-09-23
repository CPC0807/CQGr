# CQGr
Chemistry Question Generator

1.化合物元件
再題目中依照單個化合物持有資訊來建立Hypergraph
Ex. NaCl(aq)
節點

1.分子量(溶質)
2.摩爾濃度
3.重量百分濃度
4.溶解度
5.溶液質量
6.溶劑質量
7.溶質質量
8.莫耳數(溶質)
9.溶液密度

edge(無單位代表示意圖)  (會用到定理公式 及 化學反應式)
1.(Many to one)
溶液莫耳濃度 * 溶液體積 = 莫耳數
莫耳數 / 莫耳濃度 = 溶液體積
莫耳數 / 溶液體積= 溶液莫耳濃度

2.(Many to one)
溶液密度 /  溶液重量 ->溶液體積
溶液體積 * 溶液密度 ->溶液重量
溶液重量 / 溶液體積 ->密度

3.(Many to one)
莫耳數 * 分子量 -> 溶質重量
溶質重量 / 莫耳數 ->分子量
溶質重量 / 分子量 ->莫耳數

4.(Many to one)
溶質重量 / 溶液重量 -> 重量百分濃度
溶質重量 / 重量百分濃度-> 溶液重量
溶液重量 * 重量百分濃度-> 溶質重量

5.(Many to one)
溶液重量 = 溶質重量 + 溶劑
溶液重量 - 溶質重量 = 溶劑
溶液重量 - 溶劑 = 溶質重量

6.(化學反應式)
Eq. HaOH(aq) + HCl(aq) -> H2O(l) + NaCl(s)

1. 反應前化合物量
2. 反應後化合物的量
3. 反應個化合物的量
EDGE
單位統一為莫耳數

1.(Many to one)
反應前 + 反應掉 = 反應後
反應後 - 反應前 = 反應掉
反應後 - 反應掉 = 反應前

2.(One to Many)
反應掉的各化合物之間成等比關係可(1擇多)




 How to slove Word Problems


3.題型差異

在解化學反應式中，人們會將解題步驟拆解成可理解的步驟元件來進行推理。
在不同題型的的問題中，必須使用不同的Formula 及步驟找取解答。

1. 化學計量數 (Stoichiometry)
2. 濃度 (Concentrations)
3. 氣體 (Gas Laws)
4. 熱化學 (Thermochemistry)
5. 電化學 (Electrochemistry)
6. 化學平衡式 (Equilibrium)
7. 依數性（Colligative Property），是指溶液所具有的一類性質 滲透壓、溶解度
8. 熱化學（Thermochemistry）
9. 以上8種混合問題 (Miscellaneous Problems)

在上述的各式問題中，都會出現不同的演算公式及法則
必且還必須包含自然法則中所涵蓋的單位換算

d = m/V 密度公式
t = (F − 32◦)/1.8 溫度表是換算
T = t + 273◦  絕對溫度換算
KE =  1 / 2 mv2 動能物理換算
重量 = 分子量 * 莫爾數

2.濃度

M = (moles of solute)/(liter of solution) M = 溶值莫耳數 / 溶液莫耳數
m = (moles of solute)/(kilogram of solvent) m = 溶質莫耳值 / 溶液重量

3.
P1V1 = P2V2 (constant T) 分壓定理
V1/T1 = V2/T2 (constant P) 分壓定理
P1V1/T1 = P2V2/T2
PV = nRT 理想氣體方程式

Pi/ P total = ni / n total (constant V and T)
Vi/ V total = ni / n total (constant P and T)

6.
  [C]^c[D]^d
K=------------- (平衡常數)
  [A]^a[B]^b

   [A-][H+]
Ka=---------
   [HA]
   
Kw = [H+][OH-] = 1.0 x 10 ^-14

PH =  - log[H+]

將化合物資訊中的Hypergraph及化學反應式(or化學平衡式)的Hypergraph與各種公式Hypergraph相互結合。來產生各種不同的題型。
----------------------------------------------------------------------------------------------------------------------

總結:
  反應式Hypergraph + 化合物Hypergraph + 定理公式Hypergraph = 題目
 (反應式 or 平衡式)  各種化合物資訊     題型組合 
 




產生題目

1. 利用 Hypergraph 來 Check 是否擁有足夠資訊來找到解答。(REACHABILITY) 
  -所代表含意為題目有解
2. 利用 Hypergraph 來找出最少資訊就能求出的解答。(Shortest hyperpaths)


並透過結合的Hypergraph 來 Check 是否擁有足夠資訊來找到解答。(REACHABILITY)

與利用 Hypergraph 來找出最少需要多少資訊就能求出的解答。(Shortest hyperpaths)


