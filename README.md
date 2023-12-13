# Loki
Retrieval for Loki Malware Analysis 

## Commercial Antivirus Limitation

Technically, the modus operandi for the identification of malicious files and servers refers to consult in named blacklist databases. The VirusTotal platform issues the diagnoses regarding malignant characteristics related to files and web servers.

When it comes to suspicious files, VirusTotal issues the diagnostics provided by the world's leading commercial antivirus products. Regarding suspicious web servers, VirusTotal uses the database responsible for sensing virtual addresses with malicious practices.

VirusTotal has Application Programming Interface (APIs) that allow programmers to query the platform in an automated way and without the use of the graphical web interface. The proposed paper employs two of the APIs made available by VirusTotal. The first one is responsible for sending the investigated files to the platform server. The second API, in turn, makes commercial antivirus diagnostics available for files submitted to the platform by the first API.

Initially, the executable malwares are sent to the server belonging to the VirusTotal platform. After that, the executables are analyzed by the 103 commercial antiviruses linked to VirusTotal. Therefore, the antivirus provides its diagnostics for the executables submitted to the platform. VirusTotal allows the possibility of issuing three different types of diagnostics: malware, benign and omission.

Then, through the VirusTotal platform, the proposed paper investigates 103 commercial antiviruses with their respective results presented in Table 1. We used 15,675 malicious executables for 32-bit architecture. The goal of the work is to check the number of virtual pests cataloged by antivirus. The motivation is that the acquisition of new virtual plagues plays an important role in combating malicious applications. Therefore, the larger the database of malwares blacklisted, the better it tends to be the defense provided by the antivirus.

As for the first possibility of VirusTotal, the antivirus detects the malignity of the suspicious file. In the proposed experimental environment, all submitted executables are public domain malwares. Therefore, in the proposed study, the antivirus hits when it detects the malignity of the investigated executable. Malware detection indicates that the antivirus provides a robust service against cyber-intrusions. As larger the blacklist database, better tends to be the defense provided by the antivirus.

In the second possibility, the antivirus attests to the benignity of the investigated file. Therefore, in the proposed study, when the antivirus attests the benignity of the file, it is a case of a false negative – since all the samples are malicious. That is, the investigated executable is a malware; however, the antivirus attests to benignity in the wrong way.

In the third possibility, the antivirus does not emit opinion about the suspect executable. The omission indicates that the file investigated has never been evaluated by the antivirus neither it has the robustness to evaluate it in real time. The omission of the diagnosis by the antivirus points to its limitation on large-scale services.

In the third possibility, the antivirus does not emit opinion about the suspect executable. The omission indicates that the file investigated has never been evaluated by the antivirus neither it has the robustness to evaluate it in real time. The omission of the diagnosis by the antivirus points to its limitation on large-scale services.

Table 1 shows the results of the evaluated 103 antivirus products. Two of these antiviruses scored above 99%. Ten antiviruses were: MicroWorld-eScan, BitDefender, ESET-NOD32, Panda, Ad-Aware,	NANO-Antivirus,	K7AntiVirus, K7GW, Fortinet, and GData. Malware detection indicates that these antivirus programs provide a robust service against cyber-intrusions.

A major adversity in combating malicious applications is the fact that antivirus makers do not share their malware blacklists due to commercial disputes. Through Table 1 analyse, the proposed work points to an aggravating factor of this adversity: the same antivirus vendor does not even share its databases between its different antivirus programs. Note, for example, that McAfee and McAfee-GW-Edition antiviruses belong to the same company. Their blacklists, though robust, are not shared with each other. Therefore, the commercial strategies of the same company hinder the confrontation with malware. It complements that antivirus vendors are not necessarily concerned with avoiding cyber-invasions, but with optimizing their business income.

Malware detection ranged from 0% to 99.76%, depending on the antivirus being investigated. On average, the 103 antiviruses were able to detect 57.75% of the evaluated virtual pests, with a standard deviation of 41.94%. The high standard deviation indicates that the detection of malicious executables may suffer abrupt variations depending on the antivirus chosen. It is determined that the protection, against cybernetic invasions, is due to the choice of a robust antivirus with a large and updated blacklist.

As for the false negatives, the Kingsoft and CMC antiviruses wrongly stated that malware was benign in more than 90% of cases. On average, antiviruses attested false negatives in 10.11% of the cases, with a standard deviation of 20.43%. Tackling the benignity of malware can lead to irrecoverable damage. A person or institution, for example, would rely on a particular malicious application when, in fact, it is malware.

On average, the antiviruses were missing in 32.13% of the cases, with a standard deviation of 43.03%. The omission of the diagnosis points to the limitation of these antiviruses that have limited blacklists for detection of malware in real time.

It is included as adversity, in the combat to malicious applications, the fact of the commercial antiviruses do not possess a pattern in the classification of the malwares as seen in Table 2. We choose 3 of  15,675 malwares samples in order to exemplify the miscellaneous classifications of commercial antiviruses. In this way, the time when manufacturers react to a new virtual plague is affected dramatically. As there is no a pattern, antiviruses give the names that they want, for example, a company can identify a malware as "Malware.1" and a second company identify it as "Malware12310". Therefore, the lack of a pattern, besides the no-sharing of information among the antivirus manufacturers, hinders the fast and effective detection of a malicious application.


###### Table 1 Results of 103 commercial antiviruses:

Antivirus | Deteccion (%) | False Negative (%) | Omission (%)
--------- | ------------- | ------------------ | -------------
MicroWorld-eScan  |	99.76% | 0.13% |	0.11% |
BitDefender          | 99.69  % | 0.2    % | 0.11   % |
ESET-NOD32           | 99.62  % | 0.26   % | 0.13   % |
Panda                | 99.62  % | 0.34   % | 0.04   % |
Ad-Aware             | 99.51  % | 0.24   % | 0.25   % |
NANO-Antivirus       | 99.5   % | 0.32   % | 0.18   % |
K7AntiVirus          | 99.42  % | 0.52   % | 0.06   % |
K7GW                 | 99.28  % | 0.43   % | 0.29   % |
Fortinet             | 99.27  % | 0.57   % | 0.15   % |
GData                | 99.15  % | 0.34   % | 0.51   % |
McAfee               | 98.88  % | 0.79   % | 0.33   % |
AVG                  | 98.58  % | 0.19   % | 1.22   % |
AhnLab-V3            | 98.47  % | 1.5    % | 0.03   % |
Kaspersky            | 98.02  % | 1.44   % | 0.54   % |
Alibaba              | 97.91  % | 0.68   % | 1.42   % |
Microsoft            | 97.7   % | 1.85   % | 0.45   % |
DrWeb                | 97.67  % | 2.16   % | 0.18   % |
APEX                 | 97.63  % | 0.52   % | 1.84   % |
Emsisoft             | 97.42  % | 0.55   % | 2.03   % |
TrendMicro-HouseCall | 97.37  % | 2.23   % | 0.41   % |
Sophos               | 97.34  % | 1.87   % | 0.79   % |
FireEye              | 97.28  % | 0.19   % | 2.53   % |
VBA32                | 97.22  % | 2.49   % | 0.29   % |
CrowdStrike          | 97.09  % | 2.02   % | 0.89   % |
Comodo               | 96.61  % | 2.68   % | 0.71   % |
TrendMicro           | 96.3   % | 2.81   % | 0.89   % |
Avast                | 95.39  % | 2.73   % | 1.88   % |
Ikarus               | 95.17  % | 0.24   % | 4.59   % |
Cylance              | 95     % | 0.82   % | 4.18   % |
Zillya               | 94.72  % | 4.2    % | 1.08   % |
ALYac                | 94.66  % | 0.46   % | 4.88   % |
MAX                  | 94.62  % | 4.63   % | 0.76   % |
Cyren                | 94.38  % | 5.21   % | 0.41   % |
VIPRE                | 94.25  % | 4.63   % | 1.12   % |
Symantec             | 94.22  % | 1.51   % | 4.27   % |
Paloalto             | 94.19  % | 5.13   % | 0.68   % |
McAfee-GW-Edition    | 94     % | 1.88   % | 4.13   % |
Rising               | 93.77  % | 5.27   % | 0.96   % |
Cybereason           | 92.21  % | 0.58   % | 7.21   % |
Yandex               | 91.23  % | 7.92   % | 0.85   % |
Avira                | 90.6   % | 9.06   % | 0.34   % |
SentinelOne          | 89.53  % | 9.81   % | 0.66   % |
Jiangmin             | 89     % | 10.24  % | 0.76   % |
BitDefenderTheta     | 88.93  % | 1.31   % | 9.76   % |
Acronis              | 88.59  % | 9.36   % | 2.05   % |
Malwarebytes         | 86.79  % | 12.61  % | 0.61   % |
ClamAV               | 84.99  % | 13.76  % | 1.25   % |
Tencent              | 84.51  % | 14.55  % | 0.94   % |
Sangfor              | 81.8   % | 1.95   % | 16.25  % |
Lionic               | 80.76  % | 14.65  % | 4.59   % |
Zoner                | 77.81  % | 19.69  % | 2.51   % |
CAT-QuickHeal        | 75.8   % | 22.89  % | 1.31   % |
Bkav                 | 71.54  % | 26.34  % | 2.12   % |
ZoneAlarm            | 71.24  % | 27.87  % | 0.89   % |
eGambit              | 70.64  % | 13.52  % | 15.83  % |
Antiy-AVL            | 69.01  % | 28.59  % | 2.41   % |
Arcabit              | 67.54  % | 32.08  % | 0.38   % |
MaxSecure            | 67.34  % | 12.71  % | 19.96  % |
Webroot              | 64.2   % | 34.9   % | 0.9    % |
Qihoo-360            | 62.93  % | 35.32  % | 1.75   % |
Baidu                | 59.37  % | 39.51  % | 1.12   % |
Cynet                | 59.2   % | 0.09   % | 40.71  % |
Elastic              | 58.29  % | 0.22   % | 41.49  % |
F-Secure             | 51.08  % | 48.45  % | 0.47   % |
Gridinsoft           | 46.02  % | 8.26   % | 45.72  % |
Invincea             | 45.26  % | 0.28   % | 54.46  % |
TACHYON              | 41.08  % | 57.95  % | 0.96   % |
Endgame              | 40.19  % | 0.12   % | 59.69  % |
F-Prot               | 38.42  % | 2.66   % | 58.92  % |
Trapmine             | 32.85  % | 1.93   % | 65.22  % |
ViRobot              | 16.64  % | 83.27  % | 0.08   % |
SUPERAntiSpyware     | 15.78  % | 84.21  % | 0.01   % |
Kingsoft             | 2.12   % | 96.26  % | 1.63   % |
AVware               | 1.48   % | 0.04   % | 98.48  % |
nProtect             | 0.5    % | 0.4    % | 99.09  % |
Baidu-International  | 0.36   % | 0.06   % | 99.58  % |
Agnitum              | 0.33   % | 0.16   % | 99.51  % |
CMC                  | 0.33   % | 99.34  % | 0.33   % |
AntiVir              | 0.25   % | 0      % | 99.75  % |
Norman               | 0.23   % | 0.05   % | 99.72  % |
TheHacker            | 0.2    % | 1.63   % | 98.16  % |
Commtouch            | 0.2    % | 0.04   % | 99.76  % |
TotalDefense         | 0.2    % | 50.12  % | 49.68  % |
PCTools              | 0.17   % | 0.03   % | 99.81  % |
CyrenCloud           | 0.13   % | 0.01   % | 99.87  % |
VirusBuster          | 0.08   % | 0.01   % | 99.9   % |
eSafe                | 0.08   % | 0.1    % | 99.82  % |
NOD32                | 0.06   % | 0.01   % | 99.92  % |
Avast5               | 0.06   % | 0      % | 99.94  % |
ByteHero             | 0.03   % | 0.5    % | 99.48  % |
eTrust-Vet           | 0.03   % | 0.04   % | 99.92  % |
NOD32Beta            | 0.01   % | 0      % | 99.99  % |
a-squared            | 0.01   % | 0      % | 99.99  % |
McAfee+Artemis       | 0.01   % | 0      % | 99.99  % |
Kaspersky21          | 0.01   % | 0      % | 99.99  % |
Prevx                | 0.01   % | 0.07   % | 99.92  % |
BitDefenderFalx      | 0      % | 0.03   % | 99.97  % |
WhiteArmor           | 0      % | 0.06   % | 99.94  % |
Avast-Mobile         | 0      % | 40.43  % | 59.57  % |
Trustlook            | 0      % | 0.14   % | 99.86  % |
Authentium           | 0      % | 0.01   % | 99.99  % |
Sunbelt              | 0      % | 0.01   % | 99.99  % |
Babable              | 0      % | 1.33   % | 98.67  % |


###### Table 2 Miscellaneous classifications of commercial antiviruses:

Antivírus | VirusShare_001627d61a1bde3478ca4965e738dc1e | VirusShare_075efef8c9ca2f675be296d5f56406fa | VirusShare_0dab86f850fd3dafc98d0f2b401377d5
--------- | ------------------------------------------- | ------------------------------------------- | --------------------------------------------
Bkav | W32.AIDetect.malware1 | W32.AIDetect.malware1 | W32.AIDetect.malware1 |
Lionic | Trojan.Win32.Ekstak.4!c | Trojan.Win32.Ekstak.4!c | Trojan.Win32.Ekstak.4!c |
Elastic | malicious (high confidence) | malicious (high confidence) | malicious (high confidence) |
MicroWorld-eScan | Trojan.Agent.CRCF | Trojan.Agent.CRCF | Trojan.Agent.CRCF |
FireEye | Generic.mg.00019ab06b14dbd9 | Generic.mg.00009498f07e2dc9 | - |
CAT-QuickHeal | Adware.Generic.S1796222 | Trojan.Ekstak | Trojan.Ekstak |
McAfee | PWS-FCKB!00019AB06B14 | PWS-FCKB!0001B4003361 | PWS-FCKB!00009498F07E |
Cylance | Unsafe | Unsafe | Unsafe |
VIPRE | Trojan.Win32.Generic!BT | Trojan.Win32.Generic!BT | Trojan.Win32.Generic!BT |
Paloalto | generic.ml | generic.ml | generic.ml |
Sangfor | Win.Trojan.Fareit-403 | Win.Trojan.Fareit-403 | Win.Trojan.Fareit-403 |
K7AntiVirus | Trojan ( 0051e2d41 ) | Trojan ( 0051e2d41 ) | Trojan ( 0051e2d41 ) |
Alibaba | TrojanPSW:Win32/Fareit.1fde3315 | TrojanPSW:Win32/Fareit.662648ad | TrojanPSW:Win32/Fareit.fb4d3c8d |
K7GW | Trojan ( 0051e2d41 ) | Trojan ( 0051e2d41 ) | Trojan ( 0051e2d41 ) |
Cybereason | malicious.06b14d | malicious.033610 | malicious.8f07e2 |
Baidu | Win32.Trojan-PSW.Fareit.a | Win32.Trojan-PSW.Fareit.a | Win32.Trojan-PSW.Fareit.a |
Cyren | W32/Injector.ELVO-4299 | W32/Injector.ELVO-4299 | W32/Injector.ELVO-4299 |
Symantec | Trojan.Zekapab!g1 | Trojan.Zekapab!g1 | - |
ESET-NOD32 | Win32/PSW.Fareit.A | Win32/PSW.Fareit.A | Win32/PSW.Fareit.A |
APEX | Malicious | Malicious | Malicious |
Avast | Sf:Crypt-AS [Trj] | Sf:Crypt-AS [Trj] | Sf:Crypt-AS [Trj] |
ClamAV | Win.Trojan.PonyStealer-9831667-0 | None | Win.Trojan.PonyStealer-9831667-0 |
Kaspersky | HEUR:Trojan.Win32.Ekstak.gen | HEUR:Trojan.Win32.Ekstak.gen | HEUR:Trojan.Win32.Ekstak.gen |
BitDefender | Trojan.Agent.CRCF | Trojan.Agent.CRCF | Trojan.Agent.CRCF |
NANO-Antivirus | Trojan.Win32.Stealer.evlqpt | Trojan.Win32.Stealer.evlqpt | - |
SUPERAntiSpyware | None | None | None |
Rising | Stealer.Fareit!1.B777 (CLASSIC) | None | Stealer.Fareit!1.B777 (CLASSIC) |
Ad-Aware | Trojan.Agent.CRCF | Trojan.Agent.CRCF | Trojan.Agent.CRCF |
TACHYON | Trojan/W32.DP-Agent.2261177 | Trojan/W32.DP-Agent.2260975 | Trojan/W32.DP-Agent.2260999 |
Sophos | Mal/Generic-R + Troj/Delf-GOP | Mal/Generic-R + Troj/Delf-GOP | Mal/Generic-R + Troj/Delf-GOP |
Comodo | TrojWare.Win32.PWS.Fareit.DTXV@7g5m4s | TrojWare.Win32.PWS.Fareit.DTXV@7g5m4s | TrojWare.Win32.PWS.Fareit.DTXV@7g5m4s |
F-Secure | None | Dropper.DR/Delphi.vmemv | None |
DrWeb | Trojan.PWS.Stealer.18592 | Trojan.PWS.Stealer.18592 | Trojan.PWS.Stealer.18592 |
Zillya | Trojan.Ekstak.Win32.3539 | Trojan.Ekstak.Win32.3539 | Trojan.Ekstak.Win32.3539 |
TrendMicro | TSPY_HPLOKI.SM1 | TSPY_HPLOKI.SM1 | TSPY_HPLOKI.SM1 |
McAfee-GW-Edition | BehavesLike.Win32.Generic.vh | BehavesLike.Win32.Generic.vh | BehavesLike.Win32.Generic.vh |
CMC | None | None | None |
Emsisoft | Trojan.Agent.CRCF (B) | None | Trojan.Agent.CRCF (B) |
Ikarus | Trojan.Win32.Injector | Trojan.Win32.Injector | - |
GData | Trojan.Agent.CRCF | Trojan.Agent.CRCF | - |
Jiangmin | AdWare.Generic.jzzv | AdWare.Generic.jzzv | AdWare.Generic.jzzv |
Webroot | None | None | None |
Avira | None | DR/Delphi.vmemv | DR/Delphi.jdnzf |
Antiy-AVL | Trojan/Generic.ASMalwS.22D0D6F | None | - |
Kingsoft | None | None | None |
Gridinsoft | Trojan.Win32.Injector.cc!s8 | Trojan.Win32.Injector.cc!s8 | Trojan.Win32.Injector.cc!s8 |
Arcabit | None | Trojan.Agent.CRCF | None |
ViRobot | None | None | None |
ZoneAlarm | Trojan.Win32.Picsys.gen | HEUR:Trojan.Win32.Ekstak.gen | Trojan.Win32.Picsys.gen |
Microsoft | PWS:Win32/Fareit | None | PWS:Win32/Fareit |
Cynet | Malicious (score: 100) | Malicious (score: 100) | Malicious (score: 100) |
AhnLab-V3 | Trojan/Win32.Ekstak.R214290 | Trojan/Win32.Ekstak.R214290 | Trojan/Win32.Ekstak.R214290 |
Acronis | suspicious | suspicious | suspicious |
BitDefenderTheta | AI:Packer.80FC6CB421 | AI:Packer.80FC6CB421 | - |
ALYac | Trojan.Agent.CRCF | Trojan.Agent.CRCF | Trojan.Agent.CRCF |
MAX | malware (ai score=100) | malware (ai score=100) | malware (ai score=100) |
VBA32 | Trojan.Ekstak | None | BScope.Backdoor.Comet |
Malwarebytes | Pony.Spyware.Stealer.DDS | Pony.Spyware.Stealer.DDS | Pony.Spyware.Stealer.DDS |
Zoner | Trojan.Win32.63506 | Trojan.Win32.63506 | Trojan.Win32.63506 |
TrendMicro-HouseCall | TSPY_HPLOKI.SM1 | TSPY_HPLOKI.SM1 | TSPY_HPLOKI.SM1 |
Tencent | Malware.Win32.Gencirc.10b3ac7e | Malware.Win32.Gencirc.10b3ac7e | Malware.Win32.Gencirc.10b3ac7e |
Yandex | None | Trojan.GenAsa!dxedANOL6Yg | Trojan.GenAsa!dxedANOL6Yg |
SentinelOne | Static AI - Malicious PE | Static AI - Malicious PE | Static AI - Malicious PE |
eGambit | Unsafe.AI_Score_100% | Unsafe.AI_Score_100% | Unsafe.AI_Score_100% |
Fortinet | W32/GenKryptik.EKLE!tr | W32/GenKryptik.EKLE!tr | W32/GenKryptik.EKLE!tr |
MaxSecure | Trojan.Malware.300983.susgen | Trojan.Malware.121218.susgen | Trojan.Malware.121218.susgen |
AVG | Sf:Crypt-AS [Trj] | Sf:Crypt-AS [Trj] | Sf:Crypt-AS [Trj] |
Panda | Trj/Genetic.gen | Trj/Genetic.gen | Trj/Genetic.gen |
CrowdStrike | win/malicious_confidence_100% (W) | win/malicious_confidence_100% (W) | win/malicious_confidence_100% (W) |
Qihoo-360 | None | None | None |
Babable | None | - | - |
F-Prot | W32/Injector.GBX | - | - |


## Materials and Methods

This paper proposes a database aiming at the classification of 32-bit benign and malware executables. There are  15,675 malicious executables, and 3,135 other benign executables. Therefore, our dataset is suitable for learning with artificial intelligence, since both classes of executables have the same amount.

Virtual plagues were extracted from databases provided by enthusiastic study groups as VirusShare. As for benign executables, the acquisition came from benign applications repositories such as sourceforge, github and sysinternals. It should be noted that all benign executables were submitted to VirusTotal and all were its benign attested by the main commercial antivirus worldwide. The diagnostics, provided by VirusTotal, corresponding to the benign and malware executables are available in the virtual address of our database.

The purpose of the creation of the database is to give full possibility of the proposed methodology being replicated by third parties in future works. Therefore, the proposed article, by making its database freely available, enables transparency and impartiality to research, as well as demonstrating the veracity of the results achieved. Therefore, it is hoped that the methodology will serve as a basis for the creation of new scientific works.

## Executable Feature Extraction

The extraction of features of executables employs the process of disassembling. Then, the algorithm, referring to the executable, can be studied and later classified by the neural networks described in the next section. In total, 598 features of each executable are extracted, referring to the groups mentioned above. The pescanner tool are employed in order to extract the features of executables. Next, the groups of features extracted from the executables investigated are detailed.
######	Histogram of instructions, in assembly, referring to the mnemonic.
######	Number of subroutines invoking TLS (Transport Layer Security).
######	Number of subroutines responsible for exporting data (exports).  
######	APIs (Application Programming Interface) used by the executable.
######	Features related to clues that the computer has suffered fragmentation on its hard disk, as well as accumulated invalid boot attempts.  
######	Application execution mode. There are two options:
-	software with a graphical interface (GUI);
-	software running on the console.
######	Features related to the Operating System. Our digital forensics examines if the tested file tries to:
-	identify the current operating system user name;
-	access APIs in order to create and manage current OS user profiles;
-	detect the number of milliseconds since the system was initialized;
-	execute an operation in a specific file;
-	identify the version of the Windows Operating System in use;
-	monitor internal message traffic among system processes;
-	alter the Windows startup settings and contents (STARTUPINFO);  
-	allow applications to access functionality provided by shell of the operating system, as well as alter it; 
-	change the logon messages at Windows OS startup; 
-	change native applications linked to standard dialog boxes in order to open and save files, choosing color and font, among other customizations;
-	configure Windows Server licensing ; 
-	configure Windows Server 2003;
-	change the system's power settings;
-	open a process, service, or native library of the Operating System; 
-	exclude the context of certificates linked to the Operating System; 
-	copy an existing file to a new file; 
-	create, open, delete, or alter a file;
-	create and execute new process(s); 
-	create new directory(s); 
-	search for specific file(s);  
-	create a service object and add it to the control manager database for a certain service; 
-	encrypt data. It is a typical strategy of ransomwares which sequester the victim's data through cryptography. To decrypt the data, the invader asks the user for a monetary amount so that he victim can have all his data back;
-	access file systems, devices, processes, threads and error handling of the system;
-	change the sound and audio device properties of the system;
-	access graphical content information for monitors, printers, and other Windows OS output devices; 
-	use and/or monitor the USB port;
-	control a driver of a particular device; 
-	investigate if a disk drive is a removable, fixed, CD / DVD-ROM, RAM or network drive;
######	Features related to Windows Registry (Regedit). It is worth noting that the victim may not be free from malware infection even after its detection and elimination. The persistence of malefactions, even after malware exclusion, occurs due to the insertion of malicious entries (keys) in Regedit. Then, when the operating system boots, the cyber-attack restarts because of the malicious key invoking the vulnerability exploited by malware (eg: redirect Internet Explorer home page). Then, our antivirus audits if the suspicious application tries to:
-	detect the NetBIOS name of the local computer. This name is established at system startup, when the system reads it in the registry (Regedit);
-	terminate a key of a specific registry; 
-	create a key from in a specific registry. If the key already exists in Regedit, then it will be read; 
-	delete a key and its values in Regedit; 
-	enumerate and   open subkeys of a specific open registry. 
######	Features related to spywares such as keyloggers (capture of keyboard information in order to theft of passwords and logins) and screenloggers (screen shot of the victim). Our antivirus audits if the analyzed file tries to:
-	detect in which part of the victim's screen there was an update;
-	identify the screen update region by copying it to a particular region;
-	capture AVI movies and videos from web cameras and other video hardware; 
-	capture information on electronic voting, specifically from the company Optical Vote-Trakker;
-	copy an array of keyboard key states. Such strategy is typical of keyloggers
-	monitor user's Internet activity and private information;
-	collect online bank passwords and other confidential information and to send the data to invader creator;
-	access a computer from remote locations, stealing passwords, Internet banking and personal data; 
-	create a BHO (Browser Helper Object) which is executed automatically every time when the web browser is started. It fits to emphasize that BHOs are not impeded by personal firewalls because they are identified as part of the browser. In a distorted way, BHOs are often used by adware and spyware in order to record keyboard and mouse entries
-	locate passwords stored on a computer.
######	Features related to Anti-forensic Digital which are techniques of removal, occultation and subversion of evidences with the goal of reducing the consequences of the results of forensic analyzes. Our antivirus investigates if the file tries to:
-	Suspend its own execution until a certain timeout interval has elapsed. A typical malware strategy that maintains itself inactive until the end of commercial antivirus quarantine;
-	Disable the victim's defense mechanisms, including Firewall and Antivirus;
-	disable automatic Windows updates;
-	detect if the own file is being scanned by an debugger of the Operating System;   
-	retrieve information about the first and next process found in an Operating System snapshot. Such strategy is typical of malwares that aim to corrupt backups and restore points of the Operating System;
-	hide one file in another. This strategy is named, technically, steganography which aims to hide malware in a benign program in the Task Manager;
-	disguise its own name in the Task Manager;
-	make use of libraries associated with Hackers Encyclopedia 2002;
-	Create a ZeroAcess cyber-attack type through firmware updates of hardware devices (eg, hard drive controlled).
######	Features related to the creation of GUI (Graphical User Interface) of the suspicious program. Our antivirus audits if the suspect file tries to: 
-	create a GUI at runtime; 
-	use DirectX which allows multimedia applications to draw 2D graphics; 
-	create a module that contains bitmap compression and decompression routines used for Microsoft Video for Windows;
-	create 3D graphics related to utilitarian functions used by OpenGL; 
-	detect shapes through computer vision and digital image processing;
-	access functionalities in order to create and to manage screen windows and more basic controls such as buttons and scrollbars, receive mouse and keyboard input, and other functionalities associated with the Windows GUI. This includes widgets like status bars, progress bars, toolbars, and guides; 
######	Features related to the illicit forensic of the RAM (main memory) of the local system. Our antivirus investigates if the suspicious application tries to:
-	access information in specific regions of main memory;
-	read data from an area of memory occupied by a specific process;
-	write data to a memory area in a specific process;
-	reserve, confirm or alter the status of a page region in the virtual address space of a process.
######	Features related to network traffic. It is checked if the suspect file tries to:
-	query DNS servers;
-	send request to an HTTP server; 
-	monitor information of the headers of computer data packets associated with an HTTP request;
-	send an ICMP IPv4 echo request; 
-	send an SNMP request used to monitor LAN equipment;
-	terminate the Internet connection;
-	create an FTP or HTTP session at runtime; 
-	fragment a URL at runtime; 
-	query a server in order to determine the amount of traffic data available; 
-	identify the connection state of the local system in relation to the Internet; 
-	initialize the use of an application of the WinINet functions (Windows API for creating and using the application using the Internet); 
-	read data from network packets made from previous local system requests (typical behavior of sniffers); 
-	overwrite data in a local system network packet; 
-	manage local and remote network systems; 
-	create a network socket on the local system. In a conventional application, the server sends data to the client (s). In an opposite way, in malware, the victim sends the data (images, digits) to the server. Therefore, malware can create sockets on the local system waiting (listen) for a remote malicious computer to request a connection and, then, receive the victim's private information;
-	receive data of a socket. Typical strategy of backdoors when the victim starts receiving remote commands; 
-	send data to a socket. Typical strategies of spywares which, after capturing innermost information, they send them to a malicious remote computer; 
######	Features related to utility applications programs. Our created antivirus checks if the suspicious file tries to:
-	reproduce videos/audios through Windows Media Player; 
-	change the shortcut icon and Internet default settings exhibited in the Explorer toolbar address bar; 
-	alter the Wordpad configurations;
-	alter the configurations of sockets, specifically, managed by Internet Explorer; 
-	alter Outlook Express configurations and to access the victim’s  e-mail list; 
-	access information linked to the Microsof Office; 
-	alter the configurations of the Adobe System’s suite;
-	change the system's disk cleanup configurations; 
-	alter the settings of native digital electronic games and others linked to companies Tycoon and Electronic Arts;
-	change Google Inc updates settings; 
-	use Visual Basic. Such strategy is typical of macro viruses that are intended to infect applications that support macro language such as web browsers, Microsoft Office, and Adobe Systems.
-	alter the access settings to Wikipedia.
