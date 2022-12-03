Attack Surfaces of Virtual Power Plants

Crown Jewels Analysis...

Frame in terms of the Dragos 5 Critical Controls
1. ICS-specific Incident Response Plan
2. Defensible Architecture
3. Visibility and Monitoring
4. Secure Remote Access
5. Key Vulnerability Management

References:
https://arxiv.org/pdf/1907.07455.pdf
https://www.adambarth.com/papers/2011/huang-chen-barth-rescorla-jackson.pdf
https://www.coned.com/-/media/files/coned/documents/our-energy-future/our-energy-projects/distributed-system-implementation-plan.pdf
https://www.taylorfrancis.com/chapters/edit/10.1201/9781003257202-7/virtual-energy-storage-systems-virtual-power-plants-saif-sami-yue-zhou-meysam-qadrdan-jianzhong-wu
https://frost-apac.com/BDS/whitepaper/Bosch_WP.pdf
https://www.nrel.gov/docs/fy21osti/77497.pdf
https://inldigitallibrary.inl.gov/sites/sti/sti/Sort_38606.pdf
https://ieefa.org/wp-content/uploads/2022/03/What-Is-the-State-of-Virtual-Power-Plants-in-Australia_March-2022_2.pdf
https://www.rfc-editor.org/rfc/pdfrfc/rfc6455.txt.pdf
https://article.nadiapub.com/IJCA/vol10_no2/4.pdf
https://core.ac.uk/download/pdf/45601062.pdf
https://lajc.epn.edu.ec/index.php/LAJC/article/view/309
https://energy.mit.edu/wp-content/uploads/2016/04/MITEI-WP-2016-02.pdf
https://arxiv.org/ftp/arxiv/papers/2105/2105.00013.pdf
https://oa.upm.es/63128/1/TFM_JOEL_LOPEZ_SAEZ_DE_ARGANDONA.pdf
https://www.ub.tuwien.ac.at/dipl/2013/AC07815487.pdf
https://library.e.abb.com/public/75be4b6a33f046cd90c5d5aa344452e6/Cloud%20Provisioning%20Guide%20-%20ABB%20Ability%20Energy%20and%20Asset%20Manager.pdf
https://static1.squarespace.com/static/592cdfd3e6f2e1b24180305b/t/5bd1301d9140b788ed61a01b/1540436095667/deX_white_paper_FA_creating_the_grid_of_tomorrow_today+%281%29+%281%29.pdf
https://dataint.s3.amazonaws.com/media/resources/EnelX--BrianAsparro--6-27-19--ResilientPowerConf.pdf
https://www.energizeinnovation.fund/sites/default/files/2021-10/Vincent_Schachter_Enel-EPIC-Reliability-20210616.pdf

Lightbend

https://doc.akka.io/docs/akka/2.1/Akka.pdf
https://assets.ctfassets.net/sb23478ri4a9/1LVII3BSyhtTxeLRmhBary/d0817c39c594358e2a26d6e4fb587f36/akka-intro-training-public-220323102128.pdf
https://doc.akka.io/docs/akka/2.4/AkkaJava.pdf
https://mediatum.ub.tum.de/doc/1542268/pp0t4eddsgd7m1nfs5niv5wcm.Denis%20Bytschkow2.pdf
https://www.manning.com/books/akka-in-action-second-edition
https://growenergy.com.au/assets/media/Redback-Smart-HYBRID-Battery-User-Manual.pdf
https://poblliving.co.uk/wp-content/uploads/2019/09/Sonnen-Battery-Operating-Instructions.pdf

SwitchDin

https://assets.cleanenergycouncil.org.au/documents/events/WACEF-2019/4-Andrew-Mears.pdf
- SimplyEnergy as VPP Operator, SwitchDin as OEM for SA (various)
- Utility partners, product integrations, platform integrations (various)

https://static1.squarespace.com/static/592cdfd3e6f2e1b24180305b/t/6138bd68550327256e5a8d4e/1631108459969/AUSNET+Droplet+-+Fronius+Quick+Reference+Guide+V2.0.pdf
- Droplet .tar.gz firmware
- Fronius Datamanager, sometimes discoverable via Shodan. Firmware appears to be available via Fronius site
- Many CVEs identified for Fronius in general
- Default password for admin discoverable online
- Connectivity may be Inverter -> Droplet > Router, or Inverter -> Router <- Droplet
- Commissioning performed using Stormcloud by Switchdin app

https://static1.squarespace.com/static/592cdfd3e6f2e1b24180305b/t/6138bd8b73e4b665bb4cec05/1631108498965/AUSNET+Droplet+-+Growatt+Quick+Reference+Guide+V2.0.pdf
- Supports Droplet connectivity to Internet via Wifi or Ethernet
- Haptics on the device - surveillance opportunities?
- QR code-based authentication for installation - same QR code for every instance? If not, could be guessed/brute-forced?
- Can the app QR code reader be poisoned with a malicious QR code?
- Add/invite end customers - persistence?

https://static1.squarespace.com/static/592cdfd3e6f2e1b24180305b/t/5ca1407c24a6942251dd221c/1554071681513/Droplet+Industrial+v1+Brochure.pdf
- SwitchDin maintains indepedent comms - backdoor/single point of failure?
- "Connects directly	to	many	devices	for	reading	data	and	issuing	commands	using	proprietary	protocols,	SunSpec,	Modbus TCP	or	 RTU,	CAN,	Wifi.	This	includes	solar	grid	and	hybrid	inverters,	battery	management systems,	power	meters,	battery	chargers,	charge	controllers,	and	sensors." - CAN so electric vehicles?
- "Connects	to	SwitchDin	StormCloud	platform	for advanced	predictive	and	fleet-wide	control	functions for	 aggregation" - CnC

https://static1.squarespace.com/static/592cdfd3e6f2e1b24180305b/t/62d9f86a685636426094d565/1658452076223/Droplet+ONE+%7C+PLUS+info+sheet+2022+FINAL.pdf
- Droplet One vs Droplet Plus (enables 4G connectivity)
![image](https://user-images.githubusercontent.com/114399784/205427201-e09a4638-e0df-42c7-a9ed-da88b631dca7.png)

https://static1.squarespace.com/static/592cdfd3e6f2e1b24180305b/t/5f56ea31020c314b1f095f72/1599531590809/Droplet+Quick+Installation+Guide.pdf
- Older versions of SwitchDin app may be available from third party sites such as apkpure.com
https://static1.squarespace.com/static/592cdfd3e6f2e1b24180305b/t/5ca1403eec212db2221a08be/1554071617602/Droplet+Resi+v1.6+Brochure.pdf
- Remote State of Charge management
- VPP, AEMO, and NSP integration via StormCloud
- "Remote self-managed firmware upgrades using StormCloud platform" - very cool, maybe I can upload meterpreter.sh onto the device?
- "Factory fitted with X.509 certificates" - very cool - so same self-signed certificate for every Droplet device?
- "Data logging, data repair and maintenance minimises data loss" - syslog or proprietary format? Supports forwarding? In operation likely to be disabled to save storage and processing

https://static1.squarespace.com/static/592cdfd3e6f2e1b24180305b/t/5ff262a30493bd2827584e6e/1609720484842/Droplet+Resi+v1.7+Brochure+%281%29.pdf
- Basically same as 1.6 information

https://www.originenergy.com.au/wp-content/uploads/InstallManual-SI-SwitchDinInstallguide-B-IM013.pdf
- Residential droplet likes up to 40 degrees, industrial Dropet likes up to 60
- So to achieve Impact, just hog compute and persistently overheat device (no in-built fan)
- Requires connecting all inverters in same network to Droplet, which is effectively an Internet gateway. So violates Critical Control 2 (Defensible Architecture) because no segmentation/zones
- TBC

https://energycentral.com/system/files/ece/nodes/483948/is_2030.5_the_der_protocol.pdf
https://www.energy.vic.gov.au/__data/assets/pdf_file/0038/591959/Microgrid-Demonstration-Initiative-Origin-final-report.pdf

https://static1.squarespace.com/static/592cdfd3e6f2e1b24180305b/t/5ca140cf652dea0ae5655b17/1554071760320/StormCloud+v1.5a+Brochure.pdf
https://static1.squarespace.com/static/592cdfd3e6f2e1b24180305b/t/6138be845f8df85e4ea2df71/1631108743822/SAPN+Droplet+-+Fronius+Quick+Reference+Guide+V1.0.pdf
https://static1.squarespace.com/static/592cdfd3e6f2e1b24180305b/t/605348e1119d782953ab1b4d/1616070897521/SwitchDin+Droplet+Installation+and+Commissioning+V5.pdf
https://static1.squarespace.com/static/592cdfd3e6f2e1b24180305b/t/5d3630773ca1a0000166b00c/1563832442051/Utility+Resi+Droplet+Brochure+v1.0+(1).pdf

Tesla

https://fileservice.eea.comacloud.net/FileService.Api/file/FileRoom/14558058
- Megapack integrates the site controller
- Integrated thermal monitoring and management (HVAC) along with breakers - Tesla equipment or third party? Search for any mention of Schneider etc in Tesla tech docs
- Where there's lithium-ion batteries there's a target
- UL9540A: Test Method for Evaluating Thermal Runaway Fire Propagation in Battery Energy Storage Systems

https://santabarbaraca.gov/sites/default/files/filesync/Advisory_Groups/Architectural_Board_of_Review/Archive/2022_Archives/03_Architectural_Drawings/2022-03-28_March_28_2022_1150_San_Roque.pdf
https://www.osti.gov/servlets/purl/1873633
https://conference.hitb.org/hitbsecconf2021ams/materials/D1T2%20-%20X-in-the-Middle%20-%20Attacking%20Fast%20Charging%20Piles%20and%20Electric%20Vehicles%20-%20Wu%20HuiYu%20&%20Li%20Yuxiang.pdf
https://www.energy.ca.gov/sites/default/files/2021-05/CEC-500-2019-011.pdf
https://dspace.cvut.cz/bitstream/handle/10467/95016/F8-BP-2021-Sutovsky-Martin-thesis.pdf?sequence=-1
https://rickymao.me/resume.pdf
https://static1.squarespace.com/static/5becb023e17ba3fc5c907f79/t/5eac8066936c730e7e01f197/1588363372672/Tesla_Powerhub_Manual_User.pdf
https://www.gemenergy.com.au/wp-content/uploads/2017/11/Powerpack_Microgrid-System-Brochure.pdf
https://www.solarcutters.com/wp-content/uploads/2018/07/Tesla_Powerpack-System_Microgrid-Controller_v1.pdf
https://www.parliament.wa.gov.au/Parliament/commit.nsf/luInquiryPublicSubmissions/D5DFC19A737521D04825827F00261070/$file/20180413%20-%20MAT%20-%20Sub%20No.%2011%20-%20Tesla.pdf
https://www.tesla.com/sites/default/files/pdfs/en_US/Tesla-SCE-Powerpack%20Case%20Study-2017.pdf
https://energycentral.com/system/files/ece/nodes/435099/virtual_resources.pdf
https://www.infoq.com/presentations/tesla-vpp/

Aurecon
https://www.sapowernetworks.com.au/public/download.jsp?id=320260
