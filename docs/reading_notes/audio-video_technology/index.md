
# 《视频会议培训教程》读书笔记（第二部分）——视频技术和音频技术。

阅读《视频会议培训教程》这本书，所记录的笔记，此部分为第二部分。
此部分主要讲述视频技术和音频技术。
##视频技术
###H.xxx视频编码技术
-  **H.261与H.263协议**
	- H.261是最早出现的视频编码协议，目的是规范ISDN网上的会议电视和可视电话应用中的编码技术。
	- H.263协议是低码率图像压缩标准，在技术上是H.261的改进和扩充，支持码率小于64kbit/s。
	- H.261协议是视频编码的经典之作，H.263是其发展，并将逐步在实际应用中取而代之。
-  **H.264协议**
	-  H.264既是ITU-T的H.264，又是ISO/IEC的MPEG-4的第10部分。
	-  在同等图像质量下的压缩效率比以前的标准提高了2倍以上。H.264算法具有很高的编码效率，在相同的视频图像质量下，能够比H.263节约50%左右的码率。
	-  H.264的码流结构网络适应性强，增加了差错恢复能力，能够很好地适应IP和无线网络的应用。
-  **H.265协议**
	- 主要面向高清数字电视及视频编解码系统的应用，提供从SQICF至4K超高清不同级别的视频应用。
	- H.265的目标是编码效率比H.264提高50%，即在同等图像质量条件下，目标码率下降到H.264的50%。
###MPEG-X视频编码技术

-  **MPEG-1**
	- 是MPEG组织制定的第一个视频和音频有损压缩标准。
	- MPEG-1的输出质量大约和传统录像机VCR，信号质量相当。
	- MPEG-1存在诸多不足，早期用于视频监控领域。
	- **不足**：
		- 录像所要求的磁盘空间过大
		- 图像清晰度不够高
		- 对传输图像的带宽有一定的要求
		- MPEG-1的录像帧数固定为每秒25帧，不能丢帧录像，灵活性较差。

-  **MPEG-2**
	- 设计目标是高级工业标准的图像质量以及更高的传输率。 能够提供广播级的视像和CD级的音质。
	- MPEG-2除了作为DVD的制定标准外，还可用于广播、有线电视网、电缆网络以及卫星直播提供广播级的数字视频。
	- MPEG-2的另一个特点是，其可提供一个较广的范围改变压缩比，以适应不同的画面质量，存储容量，以及带宽的要求。

-  **MPEG-4**
	- 不只是具体的压缩算法，它是针对数字电视、交互式绘图应用、交互式多媒体等整合及压缩技术的需求而制定的国家标准。
	- 旨在为多媒体通信及应用环境中提供标准算法及工具，从而建立起一种能被多媒体传输、存储、检索等应用领域普遍采用的一种数据格式。
	- 主要应用于视像电话、视像电子邮件和电子新闻等
###视频编码比较

<center>

![](./image/09.png)

</center>

###视频接口
- **标清视频接口**
	- **复合视频接口**
		- 复合视频接口也叫AV接口或者Video接口是目前最普遍的一种视频接口。		
		<center>
		![](./image/10.png)
		</center>
	
	- **S-Video接口**
		
		- 为解决复合视频接口在信号重放时很难恢复与原信号完全一致的色彩的缺点，日本开发了S-Video接口
		<center>
		![](./image/11.png)
		</center>

	- **BNG接口**
		- BNG接口是指同轴电缆10Base2的接口，它用于非平衡信号的连接。

		<center>
		![](./image/12.png)
		</center>

	- **IEEE1394接口**
		- IEEE1394接口是苹果公司开发的串行标准，俗称火线接口，它支持外设热插拔，可为外设提供电源，省去了外设自带的电源，能连接多个不同设备，支持同步数据传输。
		<center>
		![](./image/13.png)
		</center>
- **标清视频接口比较** 
	<center>
	![](./image/14.png)
	</center>
- **高清视频接口**

	- **YPbPr/YCbCr色差接口**
		- 色差接口通常采用YPbPr和YCbCr两种标识，前者表示逐行扫描色差输出，后者表示隔行扫描色差输出。
		- **特点**：  
			- 由于将色度、色差分开传送，可以获得比AV端子和S端子更清晰的图像效果，而且传输距离较远。  
			- 色差分量接口是模拟接口，支持传送480I/480P/576P/4720P/1080I/1080P等格式的视	频信号，本身不传输音频信号。  
			- 色差输出的接口方式是目前最好模拟视频输出接口之一。

		<center>
		![](./image/15.png)
		</center>

	-  **VGA接口**
		-  VGA接口传输红、绿、蓝模拟信号以及同步信号，所以本质上是一种色差接口，是显卡上应用最为广泛的接口类型，也称D-Sub接口。
		-  **特点**：  
			-  VGA接口传输的仍然是模拟信号。  
			-  属于色差接口类型，所有支持传送720p/1080i/1080p等格式的视频信号。

		<center>
		![](./image/16.png)
		</center>

	-  **HDMI接口**
		-  针对DVI接口在应用中的暴露的种种问题，制定了HDMI标准。HDMI意思是高清晰多媒体接口。
		-  **特点**：  
			-  是一种数字化视频/音频接口技术，可同时传送音频和影像信号，最高数据	传输速度为48Gbps，至少支持一个1080P的视频和一个8声道的音频信号。  
			-  HDMI的设备具有“即插即用”的特点，信号源和显示设备之间会自动进行“协	商”，自动选择最合适的视频、音频格式。同时无需在信号传送前进行数/模或者模/数转换。  
			-  与DVI相比HDMI接口的体积更小，HDMI的线缆长度最假距离均不超过8米，最远传输距离不超过15米  
			-  HDMI在针脚上和DVI兼容，只是采用了不同的封装。

		<center>
		![](./image/17.png)
		</center>

	-  **DVI接口**
		-  DVI-Analog接口只传输模拟信号。  
		-  DVI-Digital接口是纯数字接口。  
		-  DVI-Integrated接口是兼容数字和模拟接口
		-  **特点**：  
			-  速度快，画面清晰。  
			-  DVI接口考虑的对象是PC，对于平板电视的兼容能力一般。  
			-  DVI接口出于兼容性考虑，预留了不少引脚以支持模拟设备，造成接口体积较大，效率低  
			-  DVI接口只能传输图像信号，对于数字音频信号的支持完全没有考虑  
			-  传输距离短，在传输带宽8Gbps情形下，传输距离为5米。
	
		<center>
		![](./image/18.png)
		</center>

	-  **SDI接口**
		-  有两种SDI标准：标准清晰度SDI和高清晰度SDI。
		-  SD-SDI与HD-SDI这两个标准的基本电气规范相同，其主要差别是HD-SDI具有更高的1.485Gbps和1.45/1001Gbps数据速率，而SD-SDI数据速率范围为143Mbps~540Mbps，最常用的是270Mbps。
		-  **HD-SDI特点**：  
			-  架设距离长，有效架设为100米  
			-  标准线缆，有效距离是100米，超过100米必须使用中继器   
			-  一根线传输，HD-SDI可以使用一根同轴电缆传输视频和音频信号。

		<center>
		![](./image/19.png)
		</center>

	-  **HDBaseT接口**
		-  接头俗称水晶头或以太网接头，传输介质采用网线， HDBaesT标准除了提供视频信号传输功能还具有网络连接以及以太网供电功能。
		-  **特点**：  
			-  支持最高20Gbps的传输速率，能完美地支持FULL 3D和4K×2K	视频格式  
			-  传输采用普通的CAT5e/6网络线缆进行无压缩传输。  
			-  连接器采用普通的RJ45接头，而传输距离到达了100米。  
			-  提供以太网功能，100W的供电能力和其他控制信号通道。 
		
		<center>
		![](./image/20.png)
		</center>
	
	- **高清视频接口比较**

	<center>
	![](./image/21.png)
	</center>
	

### 视频会议相关名词解释

- 分辨率：度量图像内数据量的多少，即屏幕图像的精密度  
- 帧率：测量显示帧数的量度  
- CIF：通用影像传输视频会议中常用的影像传输格式  
	- **特点**：
		- 在H.323协议簇中，确定其分辨率为352×288  
		- 使用NTSC帧速率，视频图像的最大帧分辨率为30幅/秒  
		- 使用1/2的PAL水平分辨率，即288线  
		- 使用逐行扫描方式  
		- 对亮度和两个色差信号（Y、Cb和Cr）分量分别进行编码  
- 隔行扫描逐行扫描：都是CRT（阴极射线管）时代显示器的水平扫描方式  
	-  **特点**：
		-  逐行扫描的图像画面平滑、无闪烁  
		-  隔行扫描行间闪烁比较明显、会造成锯齿现象  
		-  隔行扫描就是每一帧被分割成为两场，每一场包含了一帧中所有的奇数扫描行或者偶数扫描行  

###嵌入式系统

- 嵌入式系统是一个软硬件高度结合的产物，为提高执行速度和系统可靠性，嵌入式系统中的软件一般都固化在存储器芯片或单片机本身中，而不是存储于硬盘等载体中。 
- 嵌入式系统一般指非PC系统，它包括硬件和软件两部分。 
- **特点**：
	- 嵌入式系统通常是面向特定应用的  
	- 嵌入式系统CPU大多工作在特定用户群设计的系统中，具有低功耗、体积小、集成度高等特点  
	- 嵌入式系统是一个技术密集、资金密集、高度分散、不断创新的知识集成系统。  
	- 嵌入式系统的硬件和软件都必须高效率地设计，量体裁衣、去除冗余，在同样的硅片面积上实现更高的性能。  
	- 嵌入式系统具有较长的生命周期  
	- 嵌入式系统中的软件一般都固化在存储器芯片或单片机本身中
	- 用户通常不能对嵌入式系统中的程序功能进行修改，必须要有一套开发工具和环境

###双流技术

- 双流实际上是指双视频流传送技术，允许主机在一个视频会议中同时发送视频和内容。

-  **H.239双流**
	-  在一次呼叫建立媒体连接后，在两个H.239终端之间传送两路媒体流，这两条媒体流共享呼叫带宽，基于此项技术，视频用户可以得到双流视频服务，可以实现在会议系统中同时传送和显示多路视频信息。
	-  **注意**：在H.239协议中，附加的视频流是被定义为单向的，不过H.239可以允许用户容易地在会议两点之间切换发言者。

-  **“桌面传送”双流**
	-  这是一种通过插帧的方式传送静止图文的方式。桌面传送的方式实际上将其中的一帧或多帧用于传送静态图文，远程终端收到这些图像后通过VGA接口输出

###MCU会议功能
	
-  **全适配转发模式**
	-  VSW，视频转发。所有会场必须使用相同的呼叫速率，相同的视频协议、相同的分辨率，MCU不进行任何处理，类似于交换机作用，不需要额外资源板卡。

-  **全编全解模式**
	-  MCU可以将多个终端的图像进行处理、整合，然后形成一个多画面图像，再将多画面图像分别发送给不同的终端。全编全解需要MCU的额外资源板卡，各个终端可以以不同的速率、不同的分辨率、不同的视频协议进行呼叫。


###视频会议功能
<p style="text-indent:2em">
主席控制、终端自主、虚拟会议室、导演控制、自动轮询、语音激励、电话会议备份、单播、组播、短消息字幕、只能混音、码流适配、电视墙功能、多画面分割、自主多画面、数字录像和点播、数字级联、不同厂家设备互联互通
</p>
##音频技术
###音频编码技术

-  **G.711**   
	-  优点：算法复杂度低，压缩比小，编解码延时最短  
	-  缺点：占用的传输带宽较高  
-  **G.719**  
	-  优点：覆盖的音频频带上达22kHz，所占用的传输带宽低，CD级音质让声音更清晰，具有立体声能力，可对声音进行理想的跟踪  
	-  缺点：占传输带宽比较高  
-  **G.721**  
	-  优点：压缩比大  
	-  缺点：声音质量一般  
-  **G.722**  
	-  优点：音质好  
	-  缺点：占用的传输带宽较高  
-  **G.722.1**
	- 优点：音质好，占用的传输带宽已大幅下降  
	- 缺点：传输带宽仍偏高  
-  **G.722.1.C**  
	- 优点：音质更清晰，降低听着疲劳程度  
	- 缺点：是Polycom的专利技术  
-  **G.723**  
	- 优点：码率低，传输带宽要求较小。并达到ITU-TG723要求的语音质量，性能稳定  
	- 缺点：声音质量一般  
-  **G.723.1**  
	- 优点：码率低，传输带宽要求较小，并达到ITU-TG723要求的语音质量，性能稳定，避免载波信号的时通时断  
	- 缺点：声音质量一般  
-  **G.728**  
	- 优点：码率低，时延低，传输带宽占用小，采用自适应后置滤波算法提高性能  
	- 缺点：比其他编码器都复杂  
-  **G.729**  
	- 优点：传输带宽低，语音质量良，应用领域很广泛，采用矢量量化，合成分析和感觉加权，提供了对帧丢失和分组丢失的隐藏处理机制  
	- 缺点：在处理随机比特错误方面性能不好  
-  **G.729A**  
	- 优点：传输带宽低，语音质量良，降低了计算的复杂度以便于实时实现，提供了对帧丢失和分组丢失的隐藏处理机制  
	- 缺点：性能较G.729差  
-  **MPEG-1 audio layer 1**  
	- 优点：压缩方式相对于时域压缩技术要复杂很多，同时编码效率、声音质量也大幅提高，编码时延相应增加。可以达到“完全透明”的声音质量  
	- 缺点：传输带宽很高  
-  **MPEG-1  audio  layer  2**  
	- 优点：压缩方式相对时域压缩技术而言要复杂的多，同时编码效率、声音质量也大幅度提高，编码时延相应增加，可以达到“完全透明”的声音质量  
	- 缺点：传输带宽高  
-  **MPEG-1   audio  layer   3**  
	- 优点：压缩比高，适用于互联网上的传播  
	- 缺点：MP3在128Kbit及以下时，会出现明显的高频丢失  
-  **MPEG-2    audio  layer    2**  
	- 优点：支持5.1声道和7.1声道的环绕立体声    
	- 特性：以很低的传输带宽提供了低延时的高质量音频  

###音频处理技术

-  **回音抵消** 
	- 回声是由声波的反射引起的声音的重复也可指反射回来的超声波信号。  
	- AEC是回声消除器，利用它对回声进行估计，并不断地修正滤波器系数，使估计值逼近真实回音，再将估计值从话筒中减去，从而达到清除回声的目的，AEC可消除各种延迟的回声。 

-  **自动增益**
	- AGC是自动增益补偿功能，可解决声音忽大忽小的问题

-  **背景噪声消除**  
	- ANS是背景噪声抑制功能，可探测出背景固定频率的杂音并消除背景噪声。

###模拟音频接口

-  **RCA接口**  
	-  俗称莲花头，每一根RCA线缆负责传输一个声道的音频信号，一般右声道用红色标注，左声道用蓝色或者白色标注
		
	<center>![](./image/22.png)</center>

-  **小三芯，大三芯接口（TRS接口）**  
	-  用于平衡信号的传输，或者不平衡的立体声信号的传输，俗称3.5mm为小三芯，6.5mm为大三芯

	<center>
	![](./image/23.png)
	</center>

-  **卡侬接口（XLR接口）**  
	-  与RCA模拟音频线缆直接传输声音的方式完全不同，平衡音频接口使用两个通道分别传送信号相同相位相反的信号，接收端设备相减，干扰信号就被抵消  
	- 采用平衡传输方式，抵抗外界干扰能力强，利于远距离传输（不大于100米）  
	- 具有弹簧锁定装置，连接可靠，不以拉脱  
	- 接插件规定了信号流向，便于防止连接上的差错

	<center>
	![](./image/24.png)
	</center>

###数字音频接口

-  **HDMI接口**  
	- 高清晰度多媒体接口是一种数字化视频/音频接口技术，适合影像传输的专用型数字化接口，其可同时传送音频和影响信号，同时无需在信号传送前进行数/模转换或者模/数转换
	
	<center>
	![](./image/17.png)
	</center>

-  **DVI接口**  
	- DVI即数字视音频接口，是基于TMDS转换最小差分信号技术来传输数字信号。

	<center>
	![](./image/18.png)
	</center>

-  **MIC接口**  
	-  现在的数字全向麦克风通常用到此类接口，采用RJ6芯传输

	<center>
	![](./image/25.png)
	</center>

###调音台的基本功能

-  **信号放大**  
	- 调音台为适应输入信号的不同电平大小，通常在调音台输入端有高电平（线路输入）和低电平（传声输入）两个插口
-  **信号处理**  
	- 最基本的是频率均衡，根据要求对声音不同频率进行提升或衰减，以美化声源音色，也可消除噪声。
-  **信号混合**  
	- 调音台的输入有多路，而输出可能只有一路或两路，因此需要将多路信号进行混合
-  **信号分配**  
	- 调音台不仅有多路输入，还有多路输出，除主输出外，还有辅助输出和编外输出，因此需要对各路输出进行分配
-  **显示，监听，编组，遥控，对讲等功能**

	<center>
	![](./image/26.png)
	</center>

###调音台的使用

-  **信号流程**  
	- 流程图分三个部分：信号输入部分，母线部分，信号输出部分
-  **输入部分**  
	- 输入部分有13个相关部件：卡侬插座MIC，线路输入端LINE，插入插座INSERT，增益调节，均衡调节（高频段，中频段，低频段），辅助旋钮，声像调节，独奏开关，哑音开关，峰值指示灯，通道衰减器，单声道输入，立体声输入
-  **输出部分**  
	-  主输出：Main  OUTS,Main L-R,Mix  OUTS,   ST   OUTS,   ST  L-R  
	-  单声道输出：MONO OUT  
	- 主输出插入：I/O  
	- 监听输出：C-R  
	- 编组输出：SUB OUTS,  GROUP OUTS, BUS  OUTS, OMNI  OUT,   ALT  3-4  
	- 辅助输出：AUX  OUT,  AUX  SEND,  AUX1.2  
	- 直接传输：Direct  Out  
	- 录音输出:  REC  OUT  
	- 耳机输出：PHONE  

-  **幻象供电**  
	- 幻象供电就是电容调音台或前置放大器获得电源供应，通常是11～48伏的直流电，同时供应电容头的极化和放大电路的用电。各种电容麦克风耗用的电流为1～12毫安
###调音台的音频输入模式
 
-  **手拉手**  
	-  手拉手会议系统采用话筒首尾串联的连接方式，所有话筒采用幻象电源供电
	<center>
	![](./image/27.png)
	</center>

-  **一对一**  
	-  在电路结构上，传统的会议系统的话筒是放射状连接，即话筒线从调音台开始，有几只话筒就放几根话筒线接到末端的话筒上。    
	- **缺点**：围绕调音台出来的线又多又杂，易拉扯、缠绕、打结，不易管理，维修麻烦  
	- **优点**：一路话筒出现故障，不影响其他话筒使用

	<center>
	![](./image/28.png)
	</center>

[继续阅读](/reading_notes/the_construction_of_audio_and_video_system/){: .md-button }