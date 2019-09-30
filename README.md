spss统计分析
=========

## 目录
* [spss统计分析](#spss统计分析)
	* [一、spss数据整理](#一spss数据整理)
		* [1、观测量排序](#1观测量排序)
		* [2、数据的转置](#2数据的转置)
		* [3、文件合并](#3文件合并)
		* [4、数据分类汇总](#4数据分类汇总)
		* [5、数据文件分类](#5数据文件分类)
		* [6、选择数据](#6选择数据)
		* [7、数据加权](#7数据加权)
		* [8、数据的计算和变换](#8数据的计算和变换)
	* [二、spss连接数据库](#二spss连接数据库)
		* [1、odbc连接远程oracle](#1odbc连接远程oracle)
	* [三、基本统计分析](#三基本统计分析)
		* [1、频率分析](#1频率分析)
		* [2、描述分析](#2描述分析)
		* [3、探索性分析](#3探索性分析)
		* [4、交叉表分析](#4交叉表分析)
		* [5、比率分析](#5比率分析)
	* [四、均值比较分析](#四均值比较分析)
		* [1、单样本T检验](#1单样本T检验)
		* [2、独立样本T检验](#2独立样本T检验)
		* [3、成对样本T检验](#3成对样本T检验)
### 一、spss数据整理
### 1、观测量排序
- 在进行数据的处理时，有时需要按某个变量值重新排列各观测量在数据文件中出现的先后顺序<br>
1）打开SPSS软件，选择菜单栏中的【文件】→【数据】→【排序个案】命令，弹出【排序个案】对话框：<br>
2）选择排序变量，在左侧的候选变量列表框中选择主排序变量，单击右向箭头按钮，将其移动至【排序依据】列表框中。<br>
3）选择排序类型，在【排列顺序】选项组中可以选择变量排列方案。<br>
4）单击【确定】按钮，此时操作结束。<br>
![图](/data/1/1.png)
- 实例内容：地区生产总值分析<br>
地区生产总值是指某地区在一定时间内的国内生产总值，它可以作为衡量该地区经济发展的重要综合指标。准备如下图所示数据，列出了某年我国所有省、自治区、直辖市的地区生产总值及第一产业、第二产业和第三产业的生产总值，请根据这些数据分析不同省份经济发展状况的差异性<br>
![图](/data/1/1-2.png)<br>
1）选定对话框，打开SPSS软件，选择菜单栏中的【数据】→【排序个案】命令，弹出【排序个案】对话框<br>
2）选择排序变量，在左侧的候选变量列表框中选择主排序变量DQ，单击右向箭头按钮，将变量选择进入【排序依据】列表框中<br>
3）选择排序类型，为了表示不同省份生产总值的差异，按照从高到低的排列顺序，这里点选【降序】单选钮，表示观测值按照降序进行排序。<br>
4）完成操作，单击【确定】按钮，操作完成<br>
![图](/data/1/1-3.png)
### 2、数据的转置
- spss的转置功能可以将原数据文件中的行、列进行互换<br>
1）选择菜单栏中的【数据】→【转置】命令，弹出【转置】对话框<br>
2）选择转置变量，在左侧的候选变量列表框中选择需要进行转置的变量，单击右向箭头按钮，将其移动至【变量】列表框中。<br>
3）新变量命名，从左侧的候选变量列表框中可以选择一个变量，应用它的值作为转置后新变量的名称。此时，选择该变量进入  【名称变量】列表框内即可。如果用户不选择变量命名，则系统将自动给转置后的新变量赋予新的变量名。<br>
4）单击【确定】按钮，操作结束<br>
![图](/data/1/2-1.png)<br>
- 实例内容：国家财政分项目收入<br>
原财政收入数据a、b、c、d分别代表各项税收、企业亏损补贴、教育费附加收入和其他收入。根据工作需要，要将各项税收、企业亏损补贴、教育费附加收入三个变量的数据进行转置<br>
1）选择菜单栏中的【数据】→【转置】命令，弹出【转置】对话框。<br>
2）在对话框左侧的候选变量列表框中选择转置变量a、b、c，单击右向箭头按钮，将变量加入【变量】 列表框中，<br>
3）为了标识转置后新变量的意义，将左侧候选变量列表框中的【year】变量加入【名称变量】文本框中<br>
4）单击【确定】按钮完成操作<br>
![图](/data/1/2-3.png)<br>
### 3、文件合并
文件合并是指将一个外部数据文件的观测量或变量增加到当前工作文件中，将它们合并成一个文件
- 实例内容：固定资产投资文件合并<br>
原财政收入数据a、b、c、d分别代表各项税收、企业亏损补贴、教育费附加收入和其他收入。根据工作需要，要将各项税收、企业亏损补贴、教育费附加收入三个变量的数据进行转置<br>
1）选择菜单栏中的【数据】→【合并文件】→【添加个案】命令，弹出【添加个案至…】对话框<br>
2）选择合并文件，点选【外部SPSS Statistics数据文件】单选钮，同时单击【浏览】按钮，选中需要合并的文件，并指定文件路径，然后单击【继续】按钮。<br>
3）选择合并方法。<br>
4）单击【确定】按钮，操作结束<br>
![图](/data/1/3-1.png)
### 4、数据分类汇总
对数据进行分类汇总就是按指定的分类变量值对所有的观测量进行分组，对每组观测量的变量求描述统计量，并生成分组数据文件。<br>例如，将一个工厂的数据资料，按照该工厂的各个部门进行分组，并统计各个部门的人员年龄均值、方差等，这些工作就属于数据分类汇总的范畴
- 实例内容：城乡居民人民币储蓄存款<br>
- 下图是我国部分省份某年度城乡居民的人民币储蓄存款金额（年底余额,单位:亿元）。其中，“地区”变量是按地理位置对这些省份的划分，如东北地区、西南地区和西北地区等。请分析不同地区城乡居民人民币储蓄存款的差异性<br>
1）选择菜单栏中的【数据】→【汇总】命令，弹出【汇总数据】对话框。<br>
2）选择分类变量，在左侧的候选变量列表框中选择一个或多个变量作为分类变量，将其移入【分组变量】列表框中。<br>
3）选择汇总变量，在左侧的候选变量列表框中选择一个或多个变量作为汇总变量，将其移入【变量摘要】列表框中。<br>
4）选择保存类型，在【保存】选项组中点选【创建军只包含汇总变量的新数据文件】单选钮。<br>
![图](/data/1/4-1.png)<br>
### 5、数据文件分类
数据拆分是平常说的数据分组，即将数据按一个或几个分组变量分成一些供统计分析的分组，是按某种变量值重新排序
- 实例内容：分行业职工平均工资<br>
- 下图是2005年我国部分按细行业划分的职工平均工资，请根据不同的行业类型，对原始数据进行拆分，数据详见<br>
![图](/data/1/5-1.png)<br>
1）打开SPSS软件，选择菜单栏中的【数据】→【拆分文件】命令，弹出【拆分文件】对话框。<br>
2）选择数据拆分方式，点选【比较组】单选钮，表示将分组的统计结果输出到同一表格中，以此来进行不同组间的对比。<br>
3）在左侧的候选变量列表框中移动拆   分变 量“分类”至右侧的【分组方式】列表框中。<br>
4）单击【确定】按钮完成操作。<br>
![图](/data/1/5-2.png)<br>
### 6、选择数据
一般统计分析需要大量数据，但是记录中有些资料不一定全有用，根据统计目的，从数据中选取需要的作为样本参与分析
- 实例内容：城市设施水平<br>
- 下图是我国部分地区城市设施水平指标，包括城市用水普及率、城市燃气普及率等。请根据这些原始数据，选择城市用水普及率和城市燃气普及率都大于90%的地区<br>
![图](/data/1/6-1.png)<br>
1）选择菜单栏中的【数据】→【选择个案】命令，弹出【选择个案】对话框。<br>
2）点选【如果条件满足】单选钮，表示选择满足题目要求条件的观测量。单击【如果】按钮，弹出条件选择对话框。<br>
3）在上侧文本框中输入表达式“城市用水普及率＞＝0.9 & 城市用气普及率＞＝ 0.9”的条件选项，即选取城市用水普及率和城市用气普及率都大于90%的地区，单击【继续】按钮返回【选择个案】对话框。<br>
4）单击【确定】按钮完成操作。<br>
![图](/data/1/6-2.png)<br>
### 7、数据加权
- 权重的大小描述了该指标在整体评价中的相对重要程度。在数据处理中，常需要对数据进行加权处理
- 在记录有大量数据的文件中，可能同一观测量值会反复出现，如性别、民族等。如果在建立数据文件时能定义一个频数变量，也称为权重变量，用它来代表相同观测量出现的次数，这样后续的统计分析工作就会极大的简化
- 实例内容：蔬菜的平均价格<br>
- 某经销商希望掌握菜市场的蔬菜销销售的平均价格，收集数据如下图。现请利用这些数据，求出这些蔬菜的平均价格<br>
![图](/data/1/7-1.png)<br>
1）选择菜单栏中的【数据】→【个案加权】命令，弹出【个案加权】对话框。<br>
2）选择变量是否加权, 用户首先选择是否对观测量进行加权<br>
3）选择加权个案：对观测量加权，同时从左侧的候选变量列表框中选择权重变量销售量移入【频率变量】列表框中<br>
4）单击【确定】按钮完成操作。<br>
![图](/data/1/7-2.png)<br>
### 8、数据的计算和变换
- 在数据分析中，经常要根据一些已知的数据变量计算新的变量。例如，根据历年的产量数据资料计算产量的发展速度，根据人口数据计算人口出生率、死亡率等。不仅如此，还需要进行不同类型变量之间的转换，如将数值型变量转化为字符型变量。这些工作都需要利用【转换】菜单中的相关命令
- 实例内容：国内生产总值的产业构成<br>
- 收集数据如下，为我国1978-2005年国内生产总值、第一产业国内生产总值、第二产业国内生产总值和第三产业国内生产总值，请分析不同产业所占国内生产总值的变动情况<br>
![图](/data/1/8-1.png)<br>
1）打开【计算变量】对话框，打开SPSS软件，选择菜单栏中的【转换】→【计算变量】命令，弹出【计算变量】对话框<br>
2）定义目标函数名，在【目标变量】文本框中定义目标函数名为“a”，表示第一产业生产总值所占总产值的比重<br>
3）在【数值表达式】文本框中输入计算表达式“第一产业/国内生产总值”，计算第一产业生产总值所占的比重<br>
4）单击【确定】按钮，操作完成。此时，原数据文件新增加了“a”变量。<br>
![图](/data/1/8-2.png)<br>
![图](/data/1/8-3.png)<br>
### 二、spss连接数据库
### 1、odbc连接远程oracle
- 建立数据源<br>
首先通过windows的“控制面板”→“管理工具”→“ODBC数据源”，<br>
选择Oracle的数据源驱动程序，如上图所选，点击“添加”，跳出下图的对话框，<br>
“Data Source Name”填上自己设定的数据源名称，例如“spss_db”<br>
“Description”可以不写，“Home Name”选择配好的驱动，“Server” 和 “User ID”是要连接的数据库用户和密码<br>
点击“ok”，操作完成，以点击“Test Connection”(测试是否连接成功)<br>
![图](/img/1/6-1.png)<br>
- SPSS Statistics连接远程oracle数据库<br>
1) 在spss statistics打开后选择：文件→导入数据库→数据库→新建查询<br>
2) 选择上面建立好的数据源“spss_db”点下一步，跟着步骤填写，就可以添加数据库的数据了<br>
![图](/img/1/6-2.png)<br>
![图](/img/1/6-3.png)<br>
- SPSS modeler连接远程oracle数据库<br>
在“数据源”下拉对话框选上你刚刚建立的oracle的数据库连接“spss_db”，根据自己想要选择的表所在的用户，填写Oracle数据库的用户名和密码，点击“连接”即可，然后点击“确定”
然后选择所需要的表的名称，点击“确定”即可。也可以直接填写SQL查询<br>
![图](/img/1/6-4.png)<br>
- SPSS 连接mysql的方法跟上面的步骤差不多
### 三、基本统计分析
统计分析的目的是研究总体的数量特征。为实现上述分析，往往采用两种方式实现：第一，数值计算，即计算常用的基本统计量的值，通过数值来准确反映数据的基本统计特征；<br>
第二，图形绘制，即绘制常见的基本统计图形，通过图形来直观展现数据的分布特点。通常，这两种方式都是混合使用的
### 1、频率分析
- 主要能够了解变量取值的状况，对把握数据分布特征非常有用。例如，了解某班学生考试的学习成绩、了解某地区居民的收入水平等都可以借助于频数分析
- 实例内容：产品的销售量<br>
- 假设某公司每周大约卖出2000万件产品，但市场的需求不稳定，该公司的生产经理想更好的掌握近期该产品的分布情况。假设给出一批销售数字（单位：百万）代表近期公司该产品每周的销售数据。利用频数分析你能得到什么有助于
生产及销售的的信息？<br>
1）打开数据文件，选择菜单栏中的【分析】→【描述统计】→【频率】命令，弹出【频率】对话框<br>
2）在左侧的候选变量列表框中选择“sale”变量，将其添加至【变量】列表框中，表示它是进行频数分析的变量<br>
3）单击【统计量】按钮，弹出【频率：统计量】对话框；勾选【四分位数】复选框，要求输出四分数，然后单击【继续】按钮，返回【频率】对话框<br>
4）单击【图表】按钮，弹出【频率：图表】对话框，由于该数据属于数值型，因此点选【条形图】单选钮，表示结果输出条形图；再单击【继续】按钮，返回【频率】对话框<br>
5）单击【确定】按钮完成操作，输出频数分析基本统计结果，频数分析表，直方图
![图](/data/2/3-1.png)<br>
![图](/data/2/3-2.png)<br>
- 结果分析<br>
1）从基本统计表说明样本数据中有一半的数据小于20，另一半数据大于20。<br>
2）从频数分析表中可以看到，销售总量19出现的频数最多，共6次；销售总量14、17、27出现频数最小，只有1次<br>
3）从直方图形特征看，数据呈偏右分布，说明历史销售数据总体数值偏大；最大值27差不多是最小值14的一倍，说明这种产品的销售量不是很稳定，具有较大的波动性
### 2、描述分析
- 描述过程是连续资料统计描述应用最多的一个过程，它可对变量进行描述性统计分析计算，并列出一系列相应的统计指标。<br>
这和其他过程相比并无不同。该过程还有个特殊功能，就是可将原始数据转换成标准化值，并以变量的形式保存
- 实例内容：奥斯卡获奖者的年龄<br>
- 假设给出男女演员获得奥斯卡奖的年龄数据，请你分析不同性别演员获得奥斯卡奖的年龄差异性<br>
1）打开数据文件，“male”和“female”列分别表示男演员和女演员；选择菜单栏中的【分析】→【描述统计】→【描述】命令，弹出【描述性】对话框<br>
2）在左侧的候选变量列表框中选择“male”和“female”变量，将其添加至【变量】列表框中，表示它是进行描述性统计分析的变量<br>
3）单击【选项】按钮，其主要目的是选择需要输出的描述性统计量，这里除了选择系统默认的统计量外，还勾选了范围、偏度系数和峰度系数复选框；再单击【继续】按钮，返回【描述性】对话框<br>
4）单击【确定】按钮完成操作，输出结果<br>
![图](/data/2/3-3.png)<br>
- 结果分析：从输出表看出男女演员的统计人数都是36人，从样本均值看出，女演员获奖平均年龄38.94低于男演员的平均年龄45.14。男演员的范围和标准差都小于女演员，说明男演员获将年龄波动幅度小于女演员。偏度和峰度表示两组数据都不服从正态分布
### 3、探索性分析
- 探索性分析主要考察以下内容<br>
1）检查数据是否有错。过大或过小的数据均可能是异常值、影响点或错误值。要检查这样的数据，并分析原因，然后决定是否从分析中剔除这些数据。<br>
2）获得数据分布特征。很多统计方法模型对数据的分布有要求，如方差分析就需要数据服从正态分布。<br>
3）对数据的初步观察，发现一些内在规律<br>
- 实例分析：中国南北城市的温度差异<br>
- 现收集了全国主要城市2002年的年平均温度数据，试根据这些城市的南北位置差异，对其温度的差异性作探索性分析。分析南北城市的总体温度差异<br>
1）选择菜单栏中的【分析】→【描述统计】→【探索】命令，弹出【探索】对话框<br>
2）在候选变量列表框中将变量“年平均温度”添加至【因变量列表】列表框中，表示它是进行探索性分析的变量<br>
3）将变量“地域”添加至【因子列表】列表框中，表示根据地域位置不同来进行数据分析<br>
4）选择变量“城市”移入【标注个案】列表框作为标识变量，单击【统计量】按钮，在弹出的【探索：统计量】对话框中勾选【M-估计量】复选框，分析样本数据的稳定性，其他选项保持默认状态；单击【继续】按钮，返回【探索】对话框
5）单击【确定】按钮完成操作，输出结果<br>
![图](/data/2/3-4.png)<br>
- 结果分析：对比基本统计量看到，南方城市年平均气温度为18.7000，北方年平均温度11.0353。北就温度标准差3.30169大于南方温度标准差2.6880，说明北方年平均温度变化较南方更大
### 4、交叉表分析
- 是指一个频率对应两个变量的表（一个变量用来对行分类，第二个变量用来对列分类）。交叉表经常被用来分析调查结果。它有两个基本任务：<br>
第一，根据收集到的样本数据产生二维或多维交叉列联表；第二，在列联表基础上，对两两变量间是否存在一定的相关性进行分析<br>
- 实例分析：大学生身体素质调查<br>
在一次大学生身体素质的实际问卷调查，收集的主要包括：性别、出生日期、身高、体重、血型、教育背景、学科、男女身高级别和男女体重级别等内容。请根据调查数据分析下面问题：<br>
1）进行“性别”和“体重级别”双因素交叉作用下的交叉表分析，并研究“性别”对“体重级别”有无显著性影响<br>
2）进行“教育背景”和“身高级别”双因素交叉作用下的交叉表分析，并研究“教育背景”对“身高级别”有无显著性影响
- 实例操作：主要分析性别、教育背景、等因素对体重、身高等变量的数量影响关系<br>
1）打开数据，选择菜单栏中的【分析】→【描述统计】→【交叉表】命令，弹出【交叉表】对话框<br>
2）在候选变量列表框中将变量“性别（sex）”添加至【行】列表框中，表示它是交叉列联表中的行变量；将变量“体重级别（wm）”添加至【列】列表框中，表示它是交叉列联表中的列变量<br>
3）将变量“地域”添加至【因子列表】列表框中，表示根据地域位置不同来进行数据分析<br>
4）单击【统计量】按钮，弹出【交叉表：统计量】对话框，如图3-31所示；勾选【卡方】复选框，利用卡方检验来检验“性别”和“体重级别”的独立性；再单击【继续】按钮，返回【交叉表】对话框<br>
5）由于要进行“性别”和“体重级别”的频数分析，因此在【交叉表】对话框中单击【Cells（单元）】选项，弹出【交叉表：单元显示】对话框；勾选【百分比】选项组中的【行】、【列】和【总数】复选框，再单击【继续】按钮，返回【交叉表】对话框<br>
6）勾选【显示复式条形图】复选框，表示利用条形图来反映不同性别之间的体重级别差异<br>
7）单击【确定】按钮完成操作，输出结果<br>
![图](/data/2/3-5.png)<br>
- 结果分析：从交叉表可以看到，总共69名男学生中，轻体重级别有17人，中体重级别有35人，重体重级别有17人，呈对称分布特征；在所有145名女学生中，共有136名轻体重级别，数据呈左偏态，说明女生体重从总体上要低男生体重一个级别。从卡方检验概率P值都小于0.05，则拒绝零假设，认为不同性别的学生体重有显著性差异。
### 5、比率分析
- 比率分析生成比率变量，并对该比率变量计算基本描述性统计量（如均值、中位数、标准差、全距等），进而刻画出比率变量的集中趋势和离散程度。<br>
- 实例分析：城乡消费水平区域对比<br>
我国存在着显著的二元经济特征，城乡居民消费差距明显。现给出我国05年大部分省市农村居民和城镇居民的消费水平数据，利用这些数据分析我国不同区域城乡消费水平的特点<br>
- 实例操作：主要分析中国不同城乡居民消费水平的差异特点，可以区域为分组变量，利用比率分析来考察城乡居民的消费水平差距<br>
1）选择菜单栏中的【分析】→【描述统计】→【比率】命令，弹出【比值统计量】对话框<br>
2）在左侧的候选变量列表框中选取变量“城镇居民”作为比率分析的分子，将它移入右侧的【分子】列表框中<br>
3）在左侧的候选变量列表框中选取变量“农村居民”作为比率分析的分母，将它移入右侧的【分母】列表框中<br>
4）在左侧候选变量列表框中选取变量“区域”作为分组变量，将它移入右侧的【组变量】列表框中<br>
5）单击【统计量】按钮，弹出对话框；除了系统默认的输出统计量外，勾选【中位数】、【均值】和【AAD】复选框，最后单击【继续】按钮，返回【比值统计量】对话框<br>
6）单击【确定】按钮完成操作，输出结果<br>
![图](/data/2/3-6.png)<br>
- 结果分析：个案处理摘要表中，计数表示不同区域的省份数目，百分比表示不同区域省份占总体的百分比。<br>
比率表中均值和中位数表示城乡居民消费水平比率的平均值，数值越大，说明城乡消费水平差距越大。<br>
所有区域的城乡消费水平差距都大于2，说明城镇居民的消费水平是农村居民的2倍以上，反映了中国目前城乡二元经济下城乡居民生活的差距。<br>
对比不同区域，可看到西南和西北的城乡消费水平差距最大，华东、东北地区的城乡消费水平差距相对较小。平均绝对偏和离差系数等列反映了消费水平比率的离散程度。<br>
从结果看，西南地区城乡消费水平比率的离散程度最大，东北地区的离散程度最小，说明了这些不同区域内省市之间居民生活的差异性
### 四、均值比较分析
### 1、单样本T检验
- 单样本T检验的目的是利用来自某总体的样本数据，推断该总体的均值是否与指定的检验值之间存在明显的差异。它是对总体均值的假设检验。<br>
1）如果相伴概率P值小于或等于给定的显著性水平，则拒绝H0，认为总体均值与检验值之间存在显著差异。<br>
2）相反，相伴概率值大于给定的显著性水平，则不应拒绝H0，可以认为总体均值与检验值之间不存在显著差异
- 实例分析：交通通勤时间<br>
- 根据一份公共交通调查报告显示，对于那些在一个城市乘车上下班的人来说，平均通勤时间为19分钟，其人数总量为100万—300万。假设一个研究者居住在一个人口为240万的城市里，想通过验证以确定通勤时间是否和其他城市平均水平是否一致。他收集数据，随机选取了26名通勤者作为样本，假设通勤时间服从正态分布，这位研究者能得到什么结论？<br>
- 实例操作：现在该名研究者要检验他所在城市的平均通勤时间和全国其他城市平均水平是否一致。由于题目中已给出了其他城市通勤时间的平均水平为19分钟，因此，这里就是要检验该城市通勤时间是否等于19分钟
1）打开数据文件，选择菜单栏中的【分析】 →【比较均值】→【单样本T检验】命令，弹出【单样本T检验】对话框<br>
2）选择检验变量，在候选变量列表框中选择“time”变量，将其添加至【检验变量】列表框中<br>
3）选择样本检验值，在【检验值】文本框中输入检验值“19”。单击【选项】按钮，在弹出的对话框的【置信区间百分比】文本框中将系统默认的95％修改为 99％，其目的是调整显著性水平。单击【继续】按钮返回主对话框<br>
4）单击【确定】按钮完成操作，输出结果<br>
![图](/data/4/4-1.png)<br>
- 结果分析：相伴概率P值为0.471，远大于检验水平0.05，因此不拒绝原假设，不能认为样本的均值与总体均值有所不同，即判定该城市的平均通勤时间和全国水平是一致的。
### 2、独立样本T检验
- 实例分析：机场等级分数比较<br>
- 国际航空运输协会对商务旅游人员进行了一项调查，以便确定多个国际机场的等级分数。最高可能分数是10分，分数越高说明其等级也越高。假设有一个由50名商务旅行人员组成的简单随机样本，要求这些人给迈阿密机场打分。<br>
另外有一个由50名商务旅行人员组成的样本，要求这些人给洛杉矶机场打分。这两个组人员打出的等级分数。请你判断迈阿密机场和洛杉矶机场的等级评分是否相同？<br>
- 实例操作：案例中共有两组商务旅行人员分别对迈阿密和洛杉矶机场打分。由于这两组人员构成不同，因此由这两组人员组成的样本可以看作是相互独立的。<br>
现在要比较这两个机场的平均得分是否相同，也就是要检验这两个独立样本的均值是否相同，因此可以采用两独立样本t检验的方法。于是建立如下假设检验：<br>
H0 ：迈阿密机场和洛杉矶机场的等级得分相同。<br>
H1 ：迈阿密机场和洛杉矶机场的等级得分不同。<br>
1）选择菜单栏中的【分析】 →【比较均值】→【独立样本T检验】命令，弹出【独立样本T检验】对话框，。这里变量score表示两个机场的得分；变量x是不同机场的标志变量，1表示迈阿密机场，2表示洛杉矶机场<br>
2）选择检验变量，在左侧的候选变量列表框中选择检验变量“score”，将其添加至右侧的【检验变量】列表框中，表示需要对它进行独立样本的T检验<br>
3）选择分组变量，在左侧的候选变量列表框中选择分组变量“x”，将其添加至【组变量】文本框中。接着单击【定义组】按钮，弹出【定义组】对话框<br>
4）定义组别名称，点选【使用指定值】单选钮，在【组1】文本框中输入“1”，在【组2】文本框中输入“2”。输入完成后，单击【继续】按钮返回<br>
5）单击【确定】按钮完成操作，输出结果<br>
![图](/data/4/4-2.png)<br>
- 结果分析：该检验的F统计量的观察值为0.086，对应的概率P值为0.770。由于系统默认显著性水平α为0.05，而概率P值显然大于0.05，因此认为两总体的方差无显著性差异。T统计量的观测值为-0.924，对应的双尾概率P值为0.358，大于显著性水平0.05，因此认为两总体的均值不存在显著差异，即迈阿密机场和洛杉矶机场的等级得分相同。这个结论说明商务人员认为两个机场在服务水平质量等方面是没有差异的
### 3、成对样本T检验
- 成对样本T检验的目的是利用来自两个总体的配对样本，推断两个总体的均值是否存在显著差异。进行配对样本检验时，通常要满足以下三个要求。<br>
1）两组样本的样本容量要相同；<br>
2）两组样本的观察值顺序不能随意调换，要保持一一对应关系；<br>
3）样本来自的总体要服从正态分布。<br>
- 实例分析：看电视和读书的时间<br>
- 每月读书俱乐部”的成员进行了一项调查，以确信其成员用于看电视的时间是否比读书的时间多。假定抽取了15个人组成的样本，得到了有关他们每周观看电视的小时数和每周读书时间的小时数的数据。你能够得到结论：“每月读书俱乐部”的成员每周观看电视的时间比读书的时间更多吗？
- 实例操作：由于读书俱乐部的成员每人在每周可能既要看电视也要读书，因此要分析看电视和读书时间差异性，其实就是进行如下假设检验。<br>
H0 ：俱乐部成员看电视和读书所消耗的时间相同。<br>
H1 ：俱乐部成员看电视和读书所消耗的时间不同。<br>
由于抽样数据中，样本都进行了看电视和读书两个方面的时间调查，它们的活动主体都是同一个人，因此，数据类型属于配对样本的类型，故利用成对样本T检验来分析<br>
1）选择菜单栏中的【分析】 →【比较均值】→【成对样本T检验】命令，弹出【成对样本T检验】对话框。这里变量  “tv”表示成员每周看电视的时间；变量“book”表示成员每周读书的时间<br>
2）选择配对变量，在左侧的候选变量列表框中依次选择检验变量“tv”和变量“book”，将其添加至【成对变量】列表框中。这表示进行“tv”和 “book”的配对t检验<br>
3）单击【确定】按钮完成操作，输出结果<br>
![图](/data/4/4-3.png)<br>
- 结果分析：从结果来看，“tv”和“book”变量的相关系数等于0.193，呈简单正相关关系；同时相伴概率P值0.490大于显著性水平0.05说明这两组样本相关性显著。
