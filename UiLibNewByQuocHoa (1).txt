
local VexzHub = {}
VexzHub.__index = VexzHub
local Lucide = (function()
    local Icons = {
        ["a-arrow-down"] = "rbxassetid://92867583610071",
        ["a-arrow-up"] = "rbxassetid://132318504999733",
        ["a-large-small"] = "rbxassetid://111491496660216",
        ["accessibility"] = "rbxassetid://114029945302017",
        ["activity"] = "rbxassetid://94212016861936",
        ["air-vent"] = "rbxassetid://81517226012329",
        ["airplay"] = "rbxassetid://115020759309179",
        ["alarm-clock-check"] = "rbxassetid://76437352099157",
        ["alarm-clock-minus"] = "rbxassetid://77364179863205",
        ["alarm-clock-off"] = "rbxassetid://97904885874823",
        ["alarm-clock-plus"] = "rbxassetid://80468822979214",
        ["alarm-clock"] = "rbxassetid://126259032907535",
        ["alarm-smoke"] = "rbxassetid://96965448419685",
        ["album"] = "rbxassetid://127358331163602",
        ["align-center-horizontal"] = "rbxassetid://81570549209434",
        ["align-center-vertical"] = "rbxassetid://118470463752466",
        ["align-end-horizontal"] = "rbxassetid://139502909745427",
        ["align-end-vertical"] = "rbxassetid://96528869059554",
        ["align-horizontal-distribute-center"] = "rbxassetid://97220086126656",
        ["align-horizontal-distribute-end"] = "rbxassetid://106128590702022",
        ["align-horizontal-distribute-start"] = "rbxassetid://76074660002997",
        ["align-horizontal-justify-center"] = "rbxassetid://75732302772427",
        ["align-horizontal-justify-end"] = "rbxassetid://129167626402283",
        ["align-horizontal-justify-start"] = "rbxassetid://130161830325281",
        ["align-horizontal-space-around"] = "rbxassetid://91646106782950",
        ["align-horizontal-space-between"] = "rbxassetid://103886093046990",
        ["align-start-horizontal"] = "rbxassetid://125674804697729",
        ["align-start-vertical"] = "rbxassetid://105020230154823",
        ["align-vertical-distribute-center"] = "rbxassetid://93791183635525",
        ["align-vertical-distribute-end"] = "rbxassetid://139354223511433",
        ["align-vertical-distribute-start"] = "rbxassetid://74961997822126",
        ["align-vertical-justify-center"] = "rbxassetid://134754696166569",
        ["align-vertical-justify-end"] = "rbxassetid://92569381441969",
        ["align-vertical-justify-start"] = "rbxassetid://99692844572718",
        ["align-vertical-space-around"] = "rbxassetid://96206012459190",
        ["align-vertical-space-between"] = "rbxassetid://124998077349706",
        ["ambulance"] = "rbxassetid://78599995190651",
        ["ampersand"] = "rbxassetid://75272915739209",
        ["ampersands"] = "rbxassetid://126947193455996",
        ["amphora"] = "rbxassetid://137370389604364",
        ["anchor"] = "rbxassetid://92181172123618",
        ["angry"] = "rbxassetid://74237056000103",
        ["annoyed"] = "rbxassetid://80064369052011",
        ["antenna"] = "rbxassetid://99628923540956",
        ["anvil"] = "rbxassetid://100203029845919",
        ["aperture"] = "rbxassetid://83396154449972",
        ["app-window-mac"] = "rbxassetid://79587216113811",
        ["app-window"] = "rbxassetid://93142176757189",
        ["apple"] = "rbxassetid://104349242902442",
        ["archive-restore"] = "rbxassetid://78956681942188",
        ["archive-x"] = "rbxassetid://75830115088395",
        ["archive"] = "rbxassetid://122180020814574",
        ["armchair"] = "rbxassetid://105384358373973",
        ["arrow-big-down-dash"] = "rbxassetid://137987229582002",
        ["arrow-big-down"] = "rbxassetid://81081164158885",
        ["arrow-big-left-dash"] = "rbxassetid://97827621354677",
        ["arrow-big-left"] = "rbxassetid://85973092492641",
        ["arrow-big-right-dash"] = "rbxassetid://117825834972403",
        ["arrow-big-right"] = "rbxassetid://82960676755590",
        ["arrow-big-up-dash"] = "rbxassetid://99260194327483",
        ["arrow-big-up"] = "rbxassetid://93136954756149",
        ["arrow-down-0-1"] = "rbxassetid://120961896217875",
        ["arrow-down-1-0"] = "rbxassetid://93474255891850",
        ["arrow-down-a-z"] = "rbxassetid://99554596207900",
        ["arrow-down-from-line"] = "rbxassetid://132045845807798",
        ["arrow-down-left"] = "rbxassetid://102899325237364",
        ["arrow-down-narrow-wide"] = "rbxassetid://129105261655061",
        ["arrow-down-right"] = "rbxassetid://123109928624974",
        ["arrow-down-to-dot"] = "rbxassetid://101675355931221",
        ["arrow-down-to-line"] = "rbxassetid://87050478931254",
        ["arrow-down-up"] = "rbxassetid://85780258549577",
        ["arrow-down-wide-narrow"] = "rbxassetid://88461733425991",
        ["arrow-down-z-a"] = "rbxassetid://76115279362232",
        ["arrow-down"] = "rbxassetid://98764963621439",
        ["arrow-left-from-line"] = "rbxassetid://87857914437603",
        ["arrow-left-right"] = "rbxassetid://131324733048447",
        ["arrow-left-to-line"] = "rbxassetid://118645136026970",
        ["arrow-left"] = "rbxassetid://102531941843733",
        ["arrow-right-from-line"] = "rbxassetid://74073639809355",
        ["arrow-right-left"] = "rbxassetid://77015754304300",
        ["arrow-right-to-line"] = "rbxassetid://78632510329852",
        ["arrow-right"] = "rbxassetid://113692007244654",
        ["arrow-up-0-1"] = "rbxassetid://105257823943016",
        ["arrow-up-1-0"] = "rbxassetid://134175521693798",
        ["arrow-up-a-z"] = "rbxassetid://77763416595160",
        ["arrow-up-down"] = "rbxassetid://81019887641527",
        ["arrow-up-from-dot"] = "rbxassetid://124408496673275",
        ["arrow-up-from-line"] = "rbxassetid://95777664626453",
        ["arrow-up-left"] = "rbxassetid://123490598231261",
        ["arrow-up-narrow-wide"] = "rbxassetid://73006024672636",
        ["arrow-up-right"] = "rbxassetid://129280608535523",
        ["arrow-up-to-line"] = "rbxassetid://108818207813537",
        ["arrow-up-wide-narrow"] = "rbxassetid://87437426951568",
        ["arrow-up-z-a"] = "rbxassetid://107546173611884",
        ["arrow-up"] = "rbxassetid://89282378235317",
        ["arrows-up-from-line"] = "rbxassetid://133710016938621",
        ["asterisk"] = "rbxassetid://88552752106723",
        ["at-sign"] = "rbxassetid://79059152889146",
        ["atom"] = "rbxassetid://73167696981648",
        ["audio-lines"] = "rbxassetid://70930641819242",
        ["audio-waveform"] = "rbxassetid://86462036665209",
        ["award"] = "rbxassetid://132740088158419",
        ["axe"] = "rbxassetid://132405197863294",
        ["axis-3d"] = "rbxassetid://122438676546804",
        ["baby"] = "rbxassetid://93472926933440",
        ["backpack"] = "rbxassetid://140420225386018",
        ["badge-alert"] = "rbxassetid://101829200081951",
        ["badge-cent"] = "rbxassetid://133345018873154",
        ["badge-check"] = "rbxassetid://76078495178149",
        ["badge-dollar-sign"] = "rbxassetid://127139803581141",
        ["badge-euro"] = "rbxassetid://120016477674659",
        ["badge-indian-rupee"] = "rbxassetid://75659682309981",
        ["badge-info"] = "rbxassetid://131995373201472",
        ["badge-japanese-yen"] = "rbxassetid://99081574588615",
        ["badge-minus"] = "rbxassetid://140321561183881",
        ["badge-percent"] = "rbxassetid://121359224294885",
        ["badge-plus"] = "rbxassetid://100325578561866",
        ["badge-pound-sterling"] = "rbxassetid://119688217279444",
        ["badge-question-mark"] = "rbxassetid://121464963737502",
        ["badge-russian-ruble"] = "rbxassetid://108839463659864",
        ["badge-swiss-franc"] = "rbxassetid://91447608372740",
        ["badge-turkish-lira"] = "rbxassetid://137839965873529",
        ["badge-x"] = "rbxassetid://122931434733842",
        ["badge"] = "rbxassetid://116620312917084",
        ["baggage-claim"] = "rbxassetid://86922213051957",
        ["ban"] = "rbxassetid://90767043015246",
        ["banana"] = "rbxassetid://140713420056179",
        ["bandage"] = "rbxassetid://129660129590770",
        ["banknote-arrow-down"] = "rbxassetid://139366449345199",
        ["banknote-arrow-up"] = "rbxassetid://133758343082529",
        ["banknote-x"] = "rbxassetid://95348701438065",
        ["banknote"] = "rbxassetid://104840231536668",
        ["barcode"] = "rbxassetid://118473018143689",
        ["barrel"] = "rbxassetid://130647115622774",
        ["baseline"] = "rbxassetid://124677132511270",
        ["bath"] = "rbxassetid://76031400297942",
        ["battery-charging"] = "rbxassetid://80139357470047",
        ["battery-full"] = "rbxassetid://70906718268972",
        ["battery-low"] = "rbxassetid://139659256984314",
        ["battery-medium"] = "rbxassetid://105934079398915",
        ["battery-plus"] = "rbxassetid://91931341486966",
        ["battery-warning"] = "rbxassetid://115230083817257",
        ["battery"] = "rbxassetid://70765800346189",
        ["beaker"] = "rbxassetid://80902539995520",
        ["bean-off"] = "rbxassetid://98164436608714",
        ["bean"] = "rbxassetid://89491967076869",
        ["bed-double"] = "rbxassetid://73820193212911",
        ["bed-single"] = "rbxassetid://113423940880634",
        ["bed"] = "rbxassetid://97726529032925",
        ["beef"] = "rbxassetid://105850162318915",
        ["beer-off"] = "rbxassetid://120333134736361",
        ["beer"] = "rbxassetid://116404978807744",
        ["bell-dot"] = "rbxassetid://93161277118810",
        ["bell-electric"] = "rbxassetid://100277767266983",
        ["bell-minus"] = "rbxassetid://126334890449727",
        ["bell-off"] = "rbxassetid://78560046118930",
        ["bell-plus"] = "rbxassetid://77014333795836",
        ["bell-ring"] = "rbxassetid://94612128913941",
        ["bell"] = "rbxassetid://97392696311902",
        ["between-horizontal-end"] = "rbxassetid://81602774794322",
        ["between-horizontal-start"] = "rbxassetid://76112384929846",
        ["between-vertical-end"] = "rbxassetid://72817612571631",
        ["between-vertical-start"] = "rbxassetid://85278312190301",
        ["biceps-flexed"] = "rbxassetid://82004462003936",
        ["bike"] = "rbxassetid://102930322246035",
        ["binary"] = "rbxassetid://91751953950088",
        ["binoculars"] = "rbxassetid://101460003267896",
        ["biohazard"] = "rbxassetid://95956532900432",
        ["bird"] = "rbxassetid://132284145117371",
        ["birdhouse"] = "rbxassetid://83999157401433",
        ["bitcoin"] = "rbxassetid://95459240442938",
        ["blend"] = "rbxassetid://111679612185257",
        ["blinds"] = "rbxassetid://71164165283925",
        ["blocks"] = "rbxassetid://72212693357737",
        ["bluetooth-connected"] = "rbxassetid://96315134002985",
        ["bluetooth-off"] = "rbxassetid://80600044218117",
        ["bluetooth-searching"] = "rbxassetid://100673019606426",
        ["bluetooth"] = "rbxassetid://90506573139443",
        ["bold"] = "rbxassetid://116141470019166",
        ["bolt"] = "rbxassetid://102881251417484",
        ["bomb"] = "rbxassetid://139223800924636",
        ["bone"] = "rbxassetid://111242153474115",
        ["book-a"] = "rbxassetid://104067275658465",
        ["book-alert"] = "rbxassetid://124159928044853",
        ["book-audio"] = "rbxassetid://109208148317037",
        ["book-check"] = "rbxassetid://115999656081696",
        ["book-copy"] = "rbxassetid://108543407492005",
        ["book-dashed"] = "rbxassetid://127430784795958",
        ["book-down"] = "rbxassetid://101011730128222",
        ["book-headphones"] = "rbxassetid://108670200799574",
        ["book-heart"] = "rbxassetid://112788845135284",
        ["book-image"] = "rbxassetid://80808285757226",
        ["book-key"] = "rbxassetid://116024426170705",
        ["book-lock"] = "rbxassetid://118765061220571",
        ["book-marked"] = "rbxassetid://73211024251780",
        ["book-minus"] = "rbxassetid://112724962046282",
        ["book-open-check"] = "rbxassetid://130848362492667",
        ["book-open-text"] = "rbxassetid://100629528672195",
        ["book-open"] = "rbxassetid://129845326810392",
        ["book-plus"] = "rbxassetid://140267785051233",
        ["book-text"] = "rbxassetid://94011772484232",
        ["book-type"] = "rbxassetid://97817304725443",
        ["book-up-2"] = "rbxassetid://130161620853665",
        ["book-up"] = "rbxassetid://98640174079190",
        ["book-user"] = "rbxassetid://128489189240523",
        ["book-x"] = "rbxassetid://118754548186537",
        ["book"] = "rbxassetid://125383279695672",
        ["bookmark-check"] = "rbxassetid://93940443347986",
        ["bookmark-minus"] = "rbxassetid://96807096039910",
        ["bookmark-plus"] = "rbxassetid://121469724491615",
        ["bookmark-x"] = "rbxassetid://112272342584706",
        ["bookmark"] = "rbxassetid://121093149326239",
        ["boom-box"] = "rbxassetid://99901322535868",
        ["bot-message-square"] = "rbxassetid://96145330292478",
        ["bot-off"] = "rbxassetid://140417690560013",
        ["bot"] = "rbxassetid://80451686744860",
        ["bottle-wine"] = "rbxassetid://131675403196921",
        ["bow-arrow"] = "rbxassetid://124089655150375",
        ["box"] = "rbxassetid://101768155599700",
        ["boxes"] = "rbxassetid://136372617578355",
        ["braces"] = "rbxassetid://117761094704041",
        ["brackets"] = "rbxassetid://74368995728099",
        ["brain-circuit"] = "rbxassetid://70547962410202",
        ["brain-cog"] = "rbxassetid://132039205501538",
        ["brain"] = "rbxassetid://92424107303177",
        ["brick-wall-fire"] = "rbxassetid://92980588705520",
        ["brick-wall-shield"] = "rbxassetid://75954432775071",
        ["brick-wall"] = "rbxassetid://112878522258821",
        ["briefcase-business"] = "rbxassetid://129135125207283",
        ["briefcase-conveyor-belt"] = "rbxassetid://108665725653714",
        ["briefcase-medical"] = "rbxassetid://119917756334087",
        ["briefcase"] = "rbxassetid://96754188164225",
        ["bring-to-front"] = "rbxassetid://132975903553748",
        ["brush-cleaning"] = "rbxassetid://71728977448805",
        ["brush"] = "rbxassetid://127035535799640",
        ["bubbles"] = "rbxassetid://106183424168227",
        ["bug-off"] = "rbxassetid://88020025049245",
        ["bug-play"] = "rbxassetid://80107955888092",
        ["bug"] = "rbxassetid://83626408925438",
        ["building-2"] = "rbxassetid://77873775611951",
        ["building"] = "rbxassetid://110616258983082",
        ["bus-front"] = "rbxassetid://89863432456045",
        ["bus"] = "rbxassetid://133798469717463",
        ["cable-car"] = "rbxassetid://128643682205596",
        ["cable"] = "rbxassetid://128449944504901",
        ["cake-slice"] = "rbxassetid://136769828413242",
        ["cake"] = "rbxassetid://103131590503275",
        ["calculator"] = "rbxassetid://74915716529646",
        ["calendar-1"] = "rbxassetid://98458364171044",
        ["calendar-arrow-down"] = "rbxassetid://108415736543437",
        ["calendar-arrow-up"] = "rbxassetid://70574654109118",
        ["calendar-check-2"] = "rbxassetid://120231170248276",
        ["calendar-check"] = "rbxassetid://71551019465748",
        ["calendar-clock"] = "rbxassetid://119132152594595",
        ["calendar-cog"] = "rbxassetid://122402172360287",
        ["calendar-days"] = "rbxassetid://99072017568595",
        ["calendar-fold"] = "rbxassetid://117368871270394",
        ["calendar-heart"] = "rbxassetid://88839008103676",
        ["calendar-minus-2"] = "rbxassetid://98846170279891",
        ["calendar-minus"] = "rbxassetid://137354318924383",
        ["calendar-off"] = "rbxassetid://109726151749217",
        ["calendar-plus-2"] = "rbxassetid://112264562093883",
        ["calendar-plus"] = "rbxassetid://125266115249843",
        ["calendar-range"] = "rbxassetid://103641849247576",
        ["calendar-search"] = "rbxassetid://92010083223634",
        ["calendar-sync"] = "rbxassetid://78082218499697",
        ["calendar-x-2"] = "rbxassetid://107518051061147",
        ["calendar-x"] = "rbxassetid://106703374806500",
        ["calendar"] = "rbxassetid://114792700814035",
        ["camera-off"] = "rbxassetid://81057636835256",
        ["camera"] = "rbxassetid://79950339943067",
        ["candy-cane"] = "rbxassetid://71689468772492",
        ["candy-off"] = "rbxassetid://110232752314832",
        ["candy"] = "rbxassetid://107812129154678",
        ["cannabis"] = "rbxassetid://98792006538601",
        ["captions-off"] = "rbxassetid://105223545364193",
        ["captions"] = "rbxassetid://104960225031445",
        ["car-front"] = "rbxassetid://87380942739063",
        ["car-taxi-front"] = "rbxassetid://122455403384057",
        ["car"] = "rbxassetid://121065933462582",
        ["caravan"] = "rbxassetid://120070979471783",
        ["card-sim"] = "rbxassetid://134490550095771",
        ["carrot"] = "rbxassetid://119118221444304",
        ["case-lower"] = "rbxassetid://129303130603241",
        ["case-sensitive"] = "rbxassetid://125410273293056",
        ["case-upper"] = "rbxassetid://111633433531325",
        ["cassette-tape"] = "rbxassetid://137065788934157",
        ["cast"] = "rbxassetid://98202245922071",
        ["castle"] = "rbxassetid://119275077187784",
        ["cat"] = "rbxassetid://124252153404931",
        ["cctv"] = "rbxassetid://99979894766624",
        ["chart-area"] = "rbxassetid://123446436762366",
        ["chart-bar-big"] = "rbxassetid://72336824986044",
        ["chart-bar-decreasing"] = "rbxassetid://107217459044963",
        ["chart-bar-increasing"] = "rbxassetid://88268905998571",
        ["chart-bar-stacked"] = "rbxassetid://98478751113024",
        ["chart-bar"] = "rbxassetid://105389816384108",
        ["chart-candlestick"] = "rbxassetid://125676898615697",
        ["chart-column-big"] = "rbxassetid://98598733210787",
        ["chart-column-decreasing"] = "rbxassetid://73586137373563",
        ["chart-column-increasing"] = "rbxassetid://120421615068601",
        ["chart-column-stacked"] = "rbxassetid://86031449675105",
        ["chart-column"] = "rbxassetid://97915995538580",
        ["chart-gantt"] = "rbxassetid://88811660555940",
        ["chart-line"] = "rbxassetid://101833156055618",
        ["chart-network"] = "rbxassetid://104027882693561",
        ["chart-no-axes-column-decreasing"] = "rbxassetid://123371717192542",
        ["chart-no-axes-column-increasing"] = "rbxassetid://140383830943049",
        ["chart-no-axes-column"] = "rbxassetid://94078751170351",
        ["chart-no-axes-combined"] = "rbxassetid://121424233161912",
        ["chart-no-axes-gantt"] = "rbxassetid://131936541106368",
        ["chart-pie"] = "rbxassetid://113412261630136",
        ["chart-scatter"] = "rbxassetid://108217585014571",
        ["chart-spline"] = "rbxassetid://90307460742494",
        ["check-check"] = "rbxassetid://95183312173858",
        ["check-line"] = "rbxassetid://115122343485290",
        ["check"] = "rbxassetid://93898873302694",
        ["chef-hat"] = "rbxassetid://121744015002573",
        ["cherry"] = "rbxassetid://139519182403183",
        ["chess-bishop"] = "rbxassetid://121701705580238",
        ["chess-king"] = "rbxassetid://90885687223462",
        ["chess-knight"] = "rbxassetid://96467707042169",
        ["chess-pawn"] = "rbxassetid://111318574652751",
        ["chess-queen"] = "rbxassetid://98304702099749",
        ["chess-rook"] = "rbxassetid://76223925830262",
        ["chevron-down"] = "rbxassetid://134243273101015",
        ["chevron-first"] = "rbxassetid://105243363790238",
        ["chevron-last"] = "rbxassetid://89268452603731",
        ["chevron-left"] = "rbxassetid://73780377692148",
        ["chevron-right"] = "rbxassetid://92473583511724",
        ["chevron-up"] = "rbxassetid://122444883127455",
        ["chevrons-down-up"] = "rbxassetid://139404716013205",
        ["chevrons-down"] = "rbxassetid://100524612205956",
        ["chevrons-left-right-ellipsis"] = "rbxassetid://125035817741526",
        ["chevrons-left-right"] = "rbxassetid://87910685945204",
        ["chevrons-left"] = "rbxassetid://82617201744347",
        ["chevrons-right-left"] = "rbxassetid://87149546686569",
        ["chevrons-right"] = "rbxassetid://139121276490483",
        ["chevrons-up-down"] = "rbxassetid://131833120209646",
        ["chevrons-up"] = "rbxassetid://100467452364672",
        ["chromium"] = "rbxassetid://128165143739006",
        ["church"] = "rbxassetid://113714744350666",
        ["cigarette-off"] = "rbxassetid://77797883078452",
        ["circle-alert"] = "rbxassetid://83898160590116",
        ["circle-arrow-down"] = "rbxassetid://95901860261344",
        ["circle-arrow-left"] = "rbxassetid://102148876968988",
        ["circle-arrow-out-down-left"] = "rbxassetid://140598097856694",
        ["circle-arrow-out-down-right"] = "rbxassetid://119952801379305",
        ["circle-arrow-out-up-left"] = "rbxassetid://132858212688303",
        ["circle-arrow-out-up-right"] = "rbxassetid://81783743753173",
        ["circle-arrow-right"] = "rbxassetid://70786767999559",
        ["circle-arrow-up"] = "rbxassetid://84395128546494",
        ["circle-check-big"] = "rbxassetid://93202927221730",
        ["circle-check"] = "rbxassetid://85262178816537",
        ["circle-chevron-down"] = "rbxassetid://137069490345718",
        ["circle-chevron-left"] = "rbxassetid://130250009740827",
        ["circle-chevron-right"] = "rbxassetid://125943696958495",
        ["circle-chevron-up"] = "rbxassetid://111223574026321",
        ["circle-dashed"] = "rbxassetid://126799443883746",
        ["circle-divide"] = "rbxassetid://106398997754208",
        ["circle-dollar-sign"] = "rbxassetid://91106238890387",
        ["circle-dot-dashed"] = "rbxassetid://111451232827180",
        ["circle-dot"] = "rbxassetid://82947033619201",
        ["circle-ellipsis"] = "rbxassetid://91687150884779",
        ["circle-equal"] = "rbxassetid://95133963751438",
        ["circle-fading-arrow-up"] = "rbxassetid://104648212910336",
        ["circle-fading-plus"] = "rbxassetid://91847890443490",
        ["circle-gauge"] = "rbxassetid://108157549473765",
        ["circle-minus"] = "rbxassetid://133556159576809",
        ["circle-off"] = "rbxassetid://97923456918886",
        ["circle-parking-off"] = "rbxassetid://128369410981252",
        ["circle-parking"] = "rbxassetid://124034962915196",
        ["circle-pause"] = "rbxassetid://139337739700879",
        ["circle-percent"] = "rbxassetid://133311912860256",
        ["circle-play"] = "rbxassetid://120408917249739",
        ["circle-plus"] = "rbxassetid://113157136350384",
        ["circle-pound-sterling"] = "rbxassetid://105476153083828",
        ["circle-power"] = "rbxassetid://140676030155098",
        ["circle-question-mark"] = "rbxassetid://97516698664325",
        ["circle-slash-2"] = "rbxassetid://136766902186549",
        ["circle-slash"] = "rbxassetid://125206439913049",
        ["circle-small"] = "rbxassetid://73685402843600",
        ["circle-star"] = "rbxassetid://120318414957104",
        ["circle-stop"] = "rbxassetid://87400503942659",
        ["circle-user-round"] = "rbxassetid://95489465399880",
        ["circle-user"] = "rbxassetid://136220511671311",
        ["circle-x"] = "rbxassetid://76821953846248",
        ["circle"] = "rbxassetid://130359823580534",
        ["circuit-board"] = "rbxassetid://107695264369312",
        ["citrus"] = "rbxassetid://139018222976433",
        ["clapperboard"] = "rbxassetid://132660667070200",
        ["clipboard-check"] = "rbxassetid://92649798577170",
        ["clipboard-clock"] = "rbxassetid://123957515687745",
        ["clipboard-copy"] = "rbxassetid://125851897718493",
        ["clipboard-list"] = "rbxassetid://96460215958908",
        ["clipboard-minus"] = "rbxassetid://107968008485671",
        ["clipboard-paste"] = "rbxassetid://74382068849983",
        ["clipboard-pen-line"] = "rbxassetid://77711589791615",
        ["clipboard-pen"] = "rbxassetid://75290966822953",
        ["clipboard-plus"] = "rbxassetid://134285318675662",
        ["clipboard-type"] = "rbxassetid://89949374318028",
        ["clipboard-x"] = "rbxassetid://102222456890103",
        ["clipboard"] = "rbxassetid://89601995828423",
        ["clock-1"] = "rbxassetid://129363225422045",
        ["clock-10"] = "rbxassetid://104332695855541",
        ["clock-11"] = "rbxassetid://119023205186105",
        ["clock-12"] = "rbxassetid://117789618723068",
        ["clock-2"] = "rbxassetid://134710777209413",
        ["clock-3"] = "rbxassetid://136385631189327",
        ["clock-4"] = "rbxassetid://121808839832144",
        ["clock-5"] = "rbxassetid://85082019959457",
        ["clock-6"] = "rbxassetid://71009733505593",
        ["clock-7"] = "rbxassetid://103111188546225",
        ["clock-8"] = "rbxassetid://110059272125337",
        ["clock-9"] = "rbxassetid://77610027126437",
        ["clock-alert"] = "rbxassetid://97157344465162",
        ["clock-arrow-down"] = "rbxassetid://92349314416042",
        ["clock-arrow-up"] = "rbxassetid://111484286332629",
        ["clock-check"] = "rbxassetid://85231630218857",
        ["clock-fading"] = "rbxassetid://93205297285245",
        ["clock-plus"] = "rbxassetid://93367709263150",
        ["clock"] = "rbxassetid://121808839832144",
        ["closed-caption"] = "rbxassetid://99832644030788",
        ["cloud-alert"] = "rbxassetid://91967273658626",
        ["cloud-check"] = "rbxassetid://97318598202432",
        ["cloud-cog"] = "rbxassetid://96497764065749",
        ["cloud-download"] = "rbxassetid://121435581993566",
        ["cloud-drizzle"] = "rbxassetid://139525315752605",
        ["cloud-fog"] = "rbxassetid://76650233148776",
        ["cloud-hail"] = "rbxassetid://72320462748242",
        ["cloud-lightning"] = "rbxassetid://133517088924849",
        ["cloud-moon-rain"] = "rbxassetid://127667837827018",
        ["cloud-moon"] = "rbxassetid://71938114737914",
        ["cloud-off"] = "rbxassetid://131907154501444",
        ["cloud-rain-wind"] = "rbxassetid://107414583736721",
        ["cloud-rain"] = "rbxassetid://105547081967408",
        ["cloud-snow"] = "rbxassetid://72307126270226",
        ["cloud-sun-rain"] = "rbxassetid://99041604425705",
        ["cloud-sun"] = "rbxassetid://86114208148727",
        ["cloud-upload"] = "rbxassetid://93307473217005",
        ["cloud"] = "rbxassetid://121226497050352",
        ["cloudy"] = "rbxassetid://105360479023346",
        ["clover"] = "rbxassetid://74925550436750",
        ["club"] = "rbxassetid://108490365816628",
        ["code-xml"] = "rbxassetid://130150477351734",
        ["code"] = "rbxassetid://107380207681249",
        ["codepen"] = "rbxassetid://135643965971885",
        ["codesandbox"] = "rbxassetid://106911852964823",
        ["coffee"] = "rbxassetid://106864403231093",
        ["cog"] = "rbxassetid://116544501716299",
        ["coins"] = "rbxassetid://116510979641930",
        ["columns-2"] = "rbxassetid://113004100221850",
        ["columns-3-cog"] = "rbxassetid://121589691981064",
        ["columns-3"] = "rbxassetid://115223357399375",
        ["columns-4"] = "rbxassetid://130807991968419",
        ["combine"] = "rbxassetid://79908476334048",
        ["command"] = "rbxassetid://93648221906330",
        ["compass"] = "rbxassetid://115123411028382",
        ["component"] = "rbxassetid://110027788875080",
        ["computer"] = "rbxassetid://77480056459407",
        ["concierge-bell"] = "rbxassetid://140384259310436",
        ["cone"] = "rbxassetid://97759550688437",
        ["construction"] = "rbxassetid://106539489968173",
        ["contact-round"] = "rbxassetid://71907624112229",
        ["contact"] = "rbxassetid://75868297719012",
        ["container"] = "rbxassetid://91507237573499",
        ["contrast"] = "rbxassetid://112796643981497",
        ["cookie"] = "rbxassetid://73159504540002",
        ["cooking-pot"] = "rbxassetid://94959783129799",
        ["copy-check"] = "rbxassetid://91177247988892",
        ["copy-minus"] = "rbxassetid://109524509933035",
        ["copy-plus"] = "rbxassetid://113618379616952",
        ["copy-slash"] = "rbxassetid://93805787810390",
        ["copy-x"] = "rbxassetid://106557557978061",
        ["copy"] = "rbxassetid://78979572434545",
        ["copyleft"] = "rbxassetid://78559055698593",
        ["copyright"] = "rbxassetid://129433635747111",
        ["corner-down-left"] = "rbxassetid://90473561177832",
        ["corner-down-right"] = "rbxassetid://86512767702085",
        ["corner-left-down"] = "rbxassetid://139876989150630",
        ["corner-left-up"] = "rbxassetid://126228268096099",
        ["corner-right-down"] = "rbxassetid://89237035551302",
        ["corner-right-up"] = "rbxassetid://112851237026705",
        ["corner-up-left"] = "rbxassetid://84669279763024",
        ["corner-up-right"] = "rbxassetid://115099889693145",
        ["cpu"] = "rbxassetid://77549309870247",
        ["creative-commons"] = "rbxassetid://90408210735312",
        ["credit-card"] = "rbxassetid://99163352872346",
        ["croissant"] = "rbxassetid://130710485559420",
        ["crop"] = "rbxassetid://116344601101413",
        ["cross"] = "rbxassetid://101833377863588",
        ["crosshair"] = "rbxassetid://134242818164054",
        ["crown"] = "rbxassetid://127843403295538",
        ["cuboid"] = "rbxassetid://75618807946111",
        ["cup-soda"] = "rbxassetid://121098640829562",
        ["currency"] = "rbxassetid://90551250119972",
        ["cylinder"] = "rbxassetid://90569677179169",
        ["dam"] = "rbxassetid://76874486231393",
        ["database-backup"] = "rbxassetid://103403210984699",
        ["database-zap"] = "rbxassetid://131199921258418",
        ["database"] = "rbxassetid://126791525623846",
        ["decimals-arrow-left"] = "rbxassetid://120198500638749",
        ["decimals-arrow-right"] = "rbxassetid://118263047146797",
        ["delete"] = "rbxassetid://126279426372342",
        ["dessert"] = "rbxassetid://71508133278830",
        ["diameter"] = "rbxassetid://97429051503783",
        ["diamond-minus"] = "rbxassetid://128989071438290",
        ["diamond-percent"] = "rbxassetid://107717860105959",
        ["diamond-plus"] = "rbxassetid://134701163723675",
        ["diamond"] = "rbxassetid://105846996304890",
        ["dice-1"] = "rbxassetid://112650149591038",
        ["dice-2"] = "rbxassetid://112278274566793",
        ["dice-3"] = "rbxassetid://118526270626312",
        ["dice-4"] = "rbxassetid://113365650364004",
        ["dice-5"] = "rbxassetid://72768312430593",
        ["dice-6"] = "rbxassetid://85376239182543",
        ["dices"] = "rbxassetid://81268120302865",
        ["diff"] = "rbxassetid://135052708609715",
        ["disc-2"] = "rbxassetid://91419420404185",
        ["disc-3"] = "rbxassetid://135470554736048",
        ["disc-album"] = "rbxassetid://74693460404344",
        ["disc"] = "rbxassetid://101908120120777",
        ["divide"] = "rbxassetid://136678191878278",
        ["dna-off"] = "rbxassetid://89612426361540",
        ["dna"] = "rbxassetid://74007982981741",
        ["dock"] = "rbxassetid://121997427160252",
        ["dog"] = "rbxassetid://71920105558570",
        ["dollar-sign"] = "rbxassetid://127320961224019",
        ["donut"] = "rbxassetid://72204922742657",
        ["door-closed-locked"] = "rbxassetid://74027613267551",
        ["door-closed"] = "rbxassetid://136249099949073",
        ["door-open"] = "rbxassetid://91306356501736",
        ["dot"] = "rbxassetid://137321056643916",
        ["download"] = "rbxassetid://134814648082393",
        ["drafting-compass"] = "rbxassetid://99701976182841",
        ["drama"] = "rbxassetid://110297795801577",
        ["dribbble"] = "rbxassetid://80231809663849",
        ["drill"] = "rbxassetid://108644821412796",
        ["drone"] = "rbxassetid://117299095794783",
        ["droplet-off"] = "rbxassetid://119365002225172",
        ["droplet"] = "rbxassetid://100597455015098",
        ["droplets"] = "rbxassetid://140111846025180",
        ["drum"] = "rbxassetid://136979060344890",
        ["drumstick"] = "rbxassetid://104662462521709",
        ["dumbbell"] = "rbxassetid://80277236776212",
        ["ear-off"] = "rbxassetid://87421916192807",
        ["ear"] = "rbxassetid://121894949934209",
        ["earth-lock"] = "rbxassetid://88814147073745",
        ["earth"] = "rbxassetid://76231597751076",
        ["eclipse"] = "rbxassetid://114829622118222",
        ["egg-fried"] = "rbxassetid://90622538210545",
        ["egg-off"] = "rbxassetid://92288321309285",
        ["egg"] = "rbxassetid://117851493400222",
        ["ellipsis-vertical"] = "rbxassetid://117978708573781",
        ["ellipsis"] = "rbxassetid://140019550645825",
        ["equal-approximately"] = "rbxassetid://105382689698323",
        ["equal-not"] = "rbxassetid://76864449458032",
        ["equal"] = "rbxassetid://123467780715624",
        ["eraser"] = "rbxassetid://133957773112410",
        ["ethernet-port"] = "rbxassetid://75391715149314",
        ["euro"] = "rbxassetid://72229646524456",
        ["ev-charger"] = "rbxassetid://97906158859623",
        ["expand"] = "rbxassetid://137492887754537",
        ["external-link"] = "rbxassetid://129331830773832",
        ["eye-closed"] = "rbxassetid://111063268625789",
        ["eye-off"] = "rbxassetid://135928786788378",
        ["eye"] = "rbxassetid://100033680381365",
        ["facebook"] = "rbxassetid://72098528632192",
        ["factory"] = "rbxassetid://102170024318039",
        ["fan"] = "rbxassetid://78391400440696",
        ["fast-forward"] = "rbxassetid://121615540167909",
        ["feather"] = "rbxassetid://91872927606406",
        ["fence"] = "rbxassetid://123451565578029",
        ["ferris-wheel"] = "rbxassetid://79729205796176",
        ["figma"] = "rbxassetid://134182122852301",
        ["file-archive"] = "rbxassetid://77018106869967",
        ["file-axis-3d"] = "rbxassetid://133912328009885",
        ["file-badge"] = "rbxassetid://74564895394477",
        ["file-box"] = "rbxassetid://119264004071690",
        ["file-braces-corner"] = "rbxassetid://77253337986109",
        ["file-braces"] = "rbxassetid://95314128621234",
        ["file-chart-column-increasing"] = "rbxassetid://134449481172067",
        ["file-chart-column"] = "rbxassetid://82048481252560",
        ["file-chart-line"] = "rbxassetid://71954360551345",
        ["file-chart-pie"] = "rbxassetid://81072193564497",
        ["file-check-corner"] = "rbxassetid://76295552859171",
        ["file-check"] = "rbxassetid://82604001452455",
        ["file-clock"] = "rbxassetid://102325208830990",
        ["file-code-corner"] = "rbxassetid://78293841184371",
        ["file-code"] = "rbxassetid://130978036895504",
        ["file-cog"] = "rbxassetid://101385347151368",
        ["file-diff"] = "rbxassetid://96147216772241",
        ["file-digit"] = "rbxassetid://89220220354580",
        ["file-down"] = "rbxassetid://120650154178290",
        ["file-exclamation-point"] = "rbxassetid://102821865889635",
        ["file-headphone"] = "rbxassetid://100533735901986",
        ["file-heart"] = "rbxassetid://132214916401696",
        ["file-image"] = "rbxassetid://123334057511782",
        ["file-input"] = "rbxassetid://124728604166044",
        ["file-key"] = "rbxassetid://118790255921100",
        ["file-lock"] = "rbxassetid://72170228691242",
        ["file-minus-corner"] = "rbxassetid://119263271735124",
        ["file-minus"] = "rbxassetid://111014798459222",
        ["file-music"] = "rbxassetid://134948051536671",
        ["file-output"] = "rbxassetid://92146832572911",
        ["file-pen-line"] = "rbxassetid://104622936345006",
        ["file-pen"] = "rbxassetid://79556179730240",
        ["file-play"] = "rbxassetid://89006821567838",
        ["file-plus-corner"] = "rbxassetid://76544604043974",
        ["file-plus"] = "rbxassetid://78881710800060",
        ["file-question-mark"] = "rbxassetid://127617422859576",
        ["file-scan"] = "rbxassetid://129480105228213",
        ["file-search-corner"] = "rbxassetid://90974165234008",
        ["file-search"] = "rbxassetid://97780235974933",
        ["file-signal"] = "rbxassetid://122070252538165",
        ["file-sliders"] = "rbxassetid://85787771732439",
        ["file-spreadsheet"] = "rbxassetid://134501869359270",
        ["file-stack"] = "rbxassetid://138929929862605",
        ["file-symlink"] = "rbxassetid://91865722036510",
        ["file-terminal"] = "rbxassetid://116757454755476",
        ["file-text"] = "rbxassetid://90496405707281",
        ["file-type-corner"] = "rbxassetid://124902230275209",
        ["file-type"] = "rbxassetid://115272552799361",
        ["file-up"] = "rbxassetid://131173039312748",
        ["file-user"] = "rbxassetid://99552018455009",
        ["file-video-camera"] = "rbxassetid://81719056173960",
        ["file-volume"] = "rbxassetid://111264764438958",
        ["file-x-corner"] = "rbxassetid://87554136773609",
        ["file-x"] = "rbxassetid://107333775515154",
        ["file"] = "rbxassetid://74748492079329",
        ["files"] = "rbxassetid://102806336233202",
        ["film"] = "rbxassetid://120978945609706",
        ["fingerprint"] = "rbxassetid://112173305232811",
        ["fire-extinguisher"] = "rbxassetid://111643493006960",
        ["fish-off"] = "rbxassetid://89756724887508",
        ["fish-symbol"] = "rbxassetid://118475177681618",
        ["fish"] = "rbxassetid://124360663785796",
        ["flag-off"] = "rbxassetid://112944528856799",
        ["flag-triangle-left"] = "rbxassetid://88045221285272",
        ["flag-triangle-right"] = "rbxassetid://108292480304566",
        ["flag"] = "rbxassetid://78183383236196",
        ["flame-kindling"] = "rbxassetid://139728976917928",
        ["flame"] = "rbxassetid://98218034436456",
        ["flashlight-off"] = "rbxassetid://79780362871740",
        ["flashlight"] = "rbxassetid://100286985600444",
        ["flask-conical-off"] = "rbxassetid://112597970025298",
        ["flask-conical"] = "rbxassetid://128406680901165",
        ["flask-round"] = "rbxassetid://127508287324940",
        ["flip-horizontal-2"] = "rbxassetid://103726993598186",
        ["flip-horizontal"] = "rbxassetid://122937530107837",
        ["flip-vertical-2"] = "rbxassetid://103836358956328",
        ["flip-vertical"] = "rbxassetid://108003917346888",
        ["flower-2"] = "rbxassetid://72934574245145",
        ["flower"] = "rbxassetid://86129438272762",
        ["focus"] = "rbxassetid://87493973153317",
        ["fold-horizontal"] = "rbxassetid://92835712442240",
        ["fold-vertical"] = "rbxassetid://108873727253656",
        ["folder-archive"] = "rbxassetid://97312009460206",
        ["folder-check"] = "rbxassetid://128492920904557",
        ["folder-clock"] = "rbxassetid://111964836738545",
        ["folder-closed"] = "rbxassetid://118286209350843",
        ["folder-code"] = "rbxassetid://70624096349370",
        ["folder-cog"] = "rbxassetid://85299519462846",
        ["folder-dot"] = "rbxassetid://138687772725278",
        ["folder-down"] = "rbxassetid://118044108459225",
        ["folder-git-2"] = "rbxassetid://101394054141166",
        ["folder-git"] = "rbxassetid://121885778095158",
        ["folder-heart"] = "rbxassetid://79104747211105",
        ["folder-input"] = "rbxassetid://90699920697871",
        ["folder-kanban"] = "rbxassetid://78313285104072",
        ["folder-key"] = "rbxassetid://85270407596791",
        ["folder-lock"] = "rbxassetid://119201572260567",
        ["folder-minus"] = "rbxassetid://85648718999010",
        ["folder-open-dot"] = "rbxassetid://74741494767354",
        ["folder-open"] = "rbxassetid://76018996254888",
        ["folder-output"] = "rbxassetid://101532447937612",
        ["folder-pen"] = "rbxassetid://112770491173911",
        ["folder-plus"] = "rbxassetid://91865663406119",
        ["folder-root"] = "rbxassetid://103333751154693",
        ["folder-search-2"] = "rbxassetid://71276453442655",
        ["folder-search"] = "rbxassetid://110568075123861",
        ["folder-symlink"] = "rbxassetid://127485747227189",
        ["folder-sync"] = "rbxassetid://91544602659796",
        ["folder-tree"] = "rbxassetid://85577554337861",
        ["folder-up"] = "rbxassetid://72008269765857",
        ["folder-x"] = "rbxassetid://91699618247635",
        ["folder"] = "rbxassetid://80846616596607",
        ["folders"] = "rbxassetid://110351216219061",
        ["footprints"] = "rbxassetid://139192589041315",
        ["forklift"] = "rbxassetid://72030930983101",
        ["forward"] = "rbxassetid://97545944739523",
        ["frame"] = "rbxassetid://109080612832751",
        ["framer"] = "rbxassetid://108384807262391",
        ["frown"] = "rbxassetid://124407301067982",
        ["fuel"] = "rbxassetid://106447647274511",
        ["fullscreen"] = "rbxassetid://77793665526178",
        ["funnel-plus"] = "rbxassetid://100780233821928",
        ["funnel-x"] = "rbxassetid://70984385812555",
        ["funnel"] = "rbxassetid://108829540827529",
        ["gallery-horizontal-end"] = "rbxassetid://74672430161161",
        ["gallery-horizontal"] = "rbxassetid://80004001442122",
        ["gallery-thumbnails"] = "rbxassetid://136219289862706",
        ["gallery-vertical-end"] = "rbxassetid://106461402088317",
        ["gallery-vertical"] = "rbxassetid://119299431466725",
        ["gamepad-2"] = "rbxassetid://92483947987410",
        ["gamepad-directional"] = "rbxassetid://84342305212226",
        ["gamepad"] = "rbxassetid://121607283959010",
        ["gauge"] = "rbxassetid://110273524101447",
        ["gavel"] = "rbxassetid://78952298198456",
        ["gem"] = "rbxassetid://112904952151156",
        ["georgian-lari"] = "rbxassetid://98084432591687",
        ["ghost"] = "rbxassetid://113822048130017",
        ["gift"] = "rbxassetid://109855212076373",
        ["git-branch-minus"] = "rbxassetid://97385010649411",
        ["git-branch-plus"] = "rbxassetid://125944221134316",
        ["git-branch"] = "rbxassetid://90490195516649",
        ["git-commit-horizontal"] = "rbxassetid://133646041800147",
        ["git-commit-vertical"] = "rbxassetid://122098032990350",
        ["git-compare-arrows"] = "rbxassetid://84874426520216",
        ["git-compare"] = "rbxassetid://91945124438792",
        ["git-fork"] = "rbxassetid://89954992404765",
        ["git-graph"] = "rbxassetid://86166832019304",
        ["git-merge"] = "rbxassetid://131833355158059",
        ["git-pull-request-arrow"] = "rbxassetid://94507974577439",
        ["git-pull-request-closed"] = "rbxassetid://78070600389091",
        ["git-pull-request-create-arrow"] = "rbxassetid://127422677061091",
        ["git-pull-request-create"] = "rbxassetid://105929577383926",
        ["git-pull-request-draft"] = "rbxassetid://76173459869943",
        ["git-pull-request"] = "rbxassetid://138463010991471",
        ["github"] = "rbxassetid://120349554354380",
        ["gitlab"] = "rbxassetid://114054627192933",
        ["glass-water"] = "rbxassetid://115526102400988",
        ["glasses"] = "rbxassetid://87936407455373",
        ["globe-lock"] = "rbxassetid://134065526704402",
        ["globe"] = "rbxassetid://114238209622913",
        ["goal"] = "rbxassetid://120517954878160",
        ["gpu"] = "rbxassetid://95577823614219",
        ["graduation-cap"] = "rbxassetid://93771896340220",
        ["grape"] = "rbxassetid://134760640415561",
        ["grid-2x2-check"] = "rbxassetid://138468840220821",
        ["grid-2x2-plus"] = "rbxassetid://91811610580247",
        ["grid-2x2-x"] = "rbxassetid://72407303981388",
        ["grid-2x2"] = "rbxassetid://99050491897640",
        ["grid-3x2"] = "rbxassetid://95528684210010",
        ["grid-3x3"] = "rbxassetid://70419024781206",
        ["grip-horizontal"] = "rbxassetid://136255899715930",
        ["grip-vertical"] = "rbxassetid://137183678565296",
        ["grip"] = "rbxassetid://109058783556768",
        ["group"] = "rbxassetid://107643418926671",
        ["guitar"] = "rbxassetid://75915531867926",
        ["ham"] = "rbxassetid://74465607934635",
        ["hamburger"] = "rbxassetid://93086916815495",
        ["hammer"] = "rbxassetid://83545120140895",
        ["hand-coins"] = "rbxassetid://126990543175462",
        ["hand-fist"] = "rbxassetid://83341608917591",
        ["hand-grab"] = "rbxassetid://88867162163985",
        ["hand-heart"] = "rbxassetid://117507367668412",
        ["hand-helping"] = "rbxassetid://89897738419446",
        ["hand-metal"] = "rbxassetid://113619498548713",
        ["hand-platter"] = "rbxassetid://88594727743168",
        ["hand"] = "rbxassetid://130703864968637",
        ["handbag"] = "rbxassetid://135675846264061",
        ["handshake"] = "rbxassetid://78442115255814",
        ["hard-drive-download"] = "rbxassetid://73913801230614",
        ["hard-drive-upload"] = "rbxassetid://85762133615118",
        ["hard-drive"] = "rbxassetid://88183305858463",
        ["hard-hat"] = "rbxassetid://128050846767382",
        ["hash"] = "rbxassetid://82890331678520",
        ["hat-glasses"] = "rbxassetid://101165538224815",
        ["haze"] = "rbxassetid://108857561768901",
        ["hdmi-port"] = "rbxassetid://103693661037020",
        ["heading-1"] = "rbxassetid://118129315662110",
        ["heading-2"] = "rbxassetid://110209069670094",
        ["heading-3"] = "rbxassetid://90267885237062",
        ["heading-4"] = "rbxassetid://129625620307602",
        ["heading-5"] = "rbxassetid://120386663181267",
        ["heading-6"] = "rbxassetid://90959079775093",
        ["heading"] = "rbxassetid://129254312067735",
        ["headphone-off"] = "rbxassetid://85038251615641",
        ["headphones"] = "rbxassetid://118833729589183",
        ["headset"] = "rbxassetid://129269236787694",
        ["heart-crack"] = "rbxassetid://110987638564119",
        ["heart-handshake"] = "rbxassetid://111483078692002",
        ["heart-minus"] = "rbxassetid://96827380163326",
        ["heart-off"] = "rbxassetid://89748414415617",
        ["heart-plus"] = "rbxassetid://94877796283249",
        ["heart-pulse"] = "rbxassetid://129352925579546",
        ["heart"] = "rbxassetid://116559368303288",
        ["heater"] = "rbxassetid://140478466880916",
        ["helicopter"] = "rbxassetid://111557171735930",
        ["hexagon"] = "rbxassetid://127592089339199",
        ["highlighter"] = "rbxassetid://77411555641113",
        ["history"] = "rbxassetid://123980022019922",
        ["hop-off"] = "rbxassetid://103386036934034",
        ["hop"] = "rbxassetid://82778923997672",
        ["hospital"] = "rbxassetid://105868763850707",
        ["hotel"] = "rbxassetid://132283390859718",
        ["hourglass"] = "rbxassetid://86160434939203",
        ["house-heart"] = "rbxassetid://136054771868597",
        ["house-plug"] = "rbxassetid://71438263712075",
        ["house-plus"] = "rbxassetid://118495165208309",
        ["house-wifi"] = "rbxassetid://126495519725698",
        ["house"] = "rbxassetid://98755624629571",
        ["ice-cream-bowl"] = "rbxassetid://124867218454386",
        ["ice-cream-cone"] = "rbxassetid://90751397288639",
        ["id-card-lanyard"] = "rbxassetid://90761480469224",
        ["id-card"] = "rbxassetid://75354294622640",
        ["image-down"] = "rbxassetid://78972295741235",
        ["image-minus"] = "rbxassetid://101066016918565",
        ["image-off"] = "rbxassetid://81934811700938",
        ["image-play"] = "rbxassetid://129501806784210",
        ["image-plus"] = "rbxassetid://70391970623917",
        ["image-up"] = "rbxassetid://126610009605241",
        ["image-upscale"] = "rbxassetid://106963545024679",
        ["images"] = "rbxassetid://79350649395557",
        ["import"] = "rbxassetid://116545008906029",
        ["inbox"] = "rbxassetid://112591360302868",
        ["indian-rupee"] = "rbxassetid://113038778381805",
        ["infinity"] = "rbxassetid://98083086936965",
        ["info"] = "rbxassetid://124560466474914",
        ["inspection-panel"] = "rbxassetid://70905313146088",
        ["instagram"] = "rbxassetid://119864798614855",
        ["italic"] = "rbxassetid://96220378864282",
        ["iteration-ccw"] = "rbxassetid://140221832794083",
        ["iteration-cw"] = "rbxassetid://95534489554662",
        ["japanese-yen"] = "rbxassetid://106362863465813",
        ["joystick"] = "rbxassetid://99416790224739",
        ["kanban"] = "rbxassetid://125934100055431",
        ["kayak"] = "rbxassetid://136107544609389",
        ["key-round"] = "rbxassetid://83619031955390",
        ["key-square"] = "rbxassetid://94621420033649",
        ["key"] = "rbxassetid://96510194465420",
        ["keyboard-music"] = "rbxassetid://121058541758636",
        ["keyboard-off"] = "rbxassetid://92466375369772",
        ["keyboard"] = "rbxassetid://121474456068237",
        ["lamp-ceiling"] = "rbxassetid://80032758469141",
        ["lamp-desk"] = "rbxassetid://85290686983238",
        ["lamp-floor"] = "rbxassetid://104585881375892",
        ["lamp-wall-down"] = "rbxassetid://91271394132073",
        ["lamp-wall-up"] = "rbxassetid://132141464337445",
        ["lamp"] = "rbxassetid://110730830653382",
        ["land-plot"] = "rbxassetid://96449039620294",
        ["landmark"] = "rbxassetid://76885079756393",
        ["languages"] = "rbxassetid://90816903776498",
        ["laptop-minimal-check"] = "rbxassetid://114352019833865",
        ["laptop-minimal"] = "rbxassetid://136705765566068",
        ["laptop"] = "rbxassetid://111387063244975",
        ["lasso-select"] = "rbxassetid://105609719912753",
        ["lasso"] = "rbxassetid://121072936884007",
        ["laugh"] = "rbxassetid://104491311361166",
        ["layers-2"] = "rbxassetid://70536710516357",
        ["layers"] = "rbxassetid://81973586053257",
        ["layout-dashboard"] = "rbxassetid://139929981863901",
        ["layout-grid"] = "rbxassetid://81344910161871",
        ["layout-list"] = "rbxassetid://87462136296578",
        ["layout-panel-left"] = "rbxassetid://125092469751491",
        ["layout-panel-top"] = "rbxassetid://91943941515944",
        ["layout-template"] = "rbxassetid://115564446417985",
        ["leaf"] = "rbxassetid://119951075637174",
        ["leafy-green"] = "rbxassetid://105146290493154",
        ["lectern"] = "rbxassetid://106166425183862",
        ["library-big"] = "rbxassetid://106794530191412",
        ["library"] = "rbxassetid://114334671982047",
        ["life-buoy"] = "rbxassetid://81168450671956",
        ["ligature"] = "rbxassetid://111397873269411",
        ["lightbulb-off"] = "rbxassetid://83795722296178",
        ["lightbulb"] = "rbxassetid://103871245626488",
        ["line-squiggle"] = "rbxassetid://109555164424447",
        ["link-2-off"] = "rbxassetid://76885956296867",
        ["link-2"] = "rbxassetid://86072351557466",
        ["link"] = "rbxassetid://131607023382430",
        ["linkedin"] = "rbxassetid://132842789255788",
        ["list-check"] = "rbxassetid://72374358471156",
        ["list-checks"] = "rbxassetid://99809353635593",
        ["list-chevrons-down-up"] = "rbxassetid://137409641500711",
        ["list-chevrons-up-down"] = "rbxassetid://81825351389084",
        ["list-collapse"] = "rbxassetid://124505247702401",
        ["list-end"] = "rbxassetid://77650610048119",
        ["list-filter-plus"] = "rbxassetid://96385120752336",
        ["list-filter"] = "rbxassetid://103321376129527",
        ["list-indent-decrease"] = "rbxassetid://137879979228193",
        ["list-indent-increase"] = "rbxassetid://79051053161201",
        ["list-minus"] = "rbxassetid://138507965142671",
        ["list-music"] = "rbxassetid://126380635781840",
        ["list-ordered"] = "rbxassetid://83212528113913",
        ["list-plus"] = "rbxassetid://112384738137814",
        ["list-restart"] = "rbxassetid://91703153577421",
        ["list-start"] = "rbxassetid://84828348299727",
        ["list-todo"] = "rbxassetid://132980603752108",
        ["list-tree"] = "rbxassetid://97685396239010",
        ["list-video"] = "rbxassetid://93648525452489",
        ["list-x"] = "rbxassetid://113025303988861",
        ["list"] = "rbxassetid://113179976918783",
        ["loader-circle"] = "rbxassetid://116535712789945",
        ["loader-pinwheel"] = "rbxassetid://108513357940900",
        ["loader"] = "rbxassetid://78408734580845",
        ["locate-fixed"] = "rbxassetid://137367361548433",
        ["locate-off"] = "rbxassetid://73729216338137",
        ["locate"] = "rbxassetid://84467676590391",
        ["lock-keyhole-open"] = "rbxassetid://110863509313073",
        ["lock-keyhole"] = "rbxassetid://78672912777756",
        ["lock-open"] = "rbxassetid://93597915325122",
        ["lock"] = "rbxassetid://134724289526879",
        ["log-in"] = "rbxassetid://103768533135201",
        ["log-out"] = "rbxassetid://84895399304975",
        ["logs"] = "rbxassetid://89772091251787",
        ["lollipop"] = "rbxassetid://84681611583044",
        ["luggage"] = "rbxassetid://76619236486400",
        ["magnet"] = "rbxassetid://135162361226972",
        ["mail-check"] = "rbxassetid://86921536259917",
        ["mail-minus"] = "rbxassetid://81989813236553",
        ["mail-open"] = "rbxassetid://122785416858638",
        ["mail-plus"] = "rbxassetid://104886401588341",
        ["mail-question-mark"] = "rbxassetid://126540170949819",
        ["mail-search"] = "rbxassetid://135616173775287",
        ["mail-warning"] = "rbxassetid://81495303676089",
        ["mail-x"] = "rbxassetid://74607841705644",
        ["mail"] = "rbxassetid://103945161245599",
        ["mailbox"] = "rbxassetid://82765503320335",
        ["mails"] = "rbxassetid://90673453450080",
        ["map-minus"] = "rbxassetid://129525760577747",
        ["map-pin-check-inside"] = "rbxassetid://107130529843809",
        ["map-pin-check"] = "rbxassetid://118110914690154",
        ["map-pin-house"] = "rbxassetid://80546885029816",
        ["map-pin-minus-inside"] = "rbxassetid://79005529692964",
        ["map-pin-minus"] = "rbxassetid://74518762643623",
        ["map-pin-off"] = "rbxassetid://82474689391020",
        ["map-pin-pen"] = "rbxassetid://113515395277504",
        ["map-pin-plus-inside"] = "rbxassetid://134639656514430",
        ["map-pin-plus"] = "rbxassetid://91875228967029",
        ["map-pin-x-inside"] = "rbxassetid://126235934252379",
        ["map-pin-x"] = "rbxassetid://101085273547316",
        ["map-pin"] = "rbxassetid://84279202219901",
        ["map-pinned"] = "rbxassetid://103963788475034",
        ["map-plus"] = "rbxassetid://129388826743495",
        ["map"] = "rbxassetid://95107167260947",
        ["mars-stroke"] = "rbxassetid://131973193186828",
        ["mars"] = "rbxassetid://111287112372511",
        ["martini"] = "rbxassetid://82977695401058",
        ["maximize-2"] = "rbxassetid://73085922906397",
        ["maximize"] = "rbxassetid://76045941763188",
        ["medal"] = "rbxassetid://79016002264450",
        ["megaphone-off"] = "rbxassetid://124280774193935",
        ["megaphone"] = "rbxassetid://118759541854879",
        ["meh"] = "rbxassetid://132197867028557",
        ["memory-stick"] = "rbxassetid://93212591343119",
        ["menu"] = "rbxassetid://77021539815611",
        ["merge"] = "rbxassetid://126201866476775",
        ["message-circle-code"] = "rbxassetid://112865244991651",
        ["message-circle-dashed"] = "rbxassetid://81525157881897",
        ["message-circle-heart"] = "rbxassetid://101990756073677",
        ["message-circle-more"] = "rbxassetid://92856823884663",
        ["message-circle-off"] = "rbxassetid://134955643890328",
        ["message-circle-plus"] = "rbxassetid://106562979649273",
        ["message-circle-question-mark"] = "rbxassetid://107700302759934",
        ["message-circle-reply"] = "rbxassetid://137071749508334",
        ["message-circle-warning"] = "rbxassetid://119020096067894",
        ["message-circle-x"] = "rbxassetid://126843387725536",
        ["message-circle"] = "rbxassetid://127255077587058",
        ["message-square-code"] = "rbxassetid://110968863152123",
        ["message-square-dashed"] = "rbxassetid://107653455516238",
        ["message-square-diff"] = "rbxassetid://75472190472625",
        ["message-square-dot"] = "rbxassetid://127806382463916",
        ["message-square-heart"] = "rbxassetid://75612811742074",
        ["message-square-lock"] = "rbxassetid://81268215619563",
        ["message-square-more"] = "rbxassetid://120139782405970",
        ["message-square-off"] = "rbxassetid://99961019005789",
        ["message-square-plus"] = "rbxassetid://76934450256199",
        ["message-square-quote"] = "rbxassetid://116670768629340",
        ["message-square-reply"] = "rbxassetid://130985622754637",
        ["message-square-share"] = "rbxassetid://131017005324026",
        ["message-square-text"] = "rbxassetid://94899503194205",
        ["message-square-warning"] = "rbxassetid://138432903962261",
        ["message-square-x"] = "rbxassetid://137285463279462",
        ["message-square"] = "rbxassetid://83881670383280",
        ["messages-square"] = "rbxassetid://97532166733358",
        ["mic-off"] = "rbxassetid://82123034444822",
        ["mic-vocal"] = "rbxassetid://99082286164362",
        ["mic"] = "rbxassetid://89640799126523",
        ["microchip"] = "rbxassetid://73937907669903",
        ["microscope"] = "rbxassetid://116875530102782",
        ["microwave"] = "rbxassetid://108411735353008",
        ["milestone"] = "rbxassetid://101618292325920",
        ["milk-off"] = "rbxassetid://72388480962742",
        ["milk"] = "rbxassetid://96221903896918",
        ["minimize-2"] = "rbxassetid://116269596042539",
        ["minimize"] = "rbxassetid://121304296213645",
        ["minus"] = "rbxassetid://118026365011536",
        ["monitor-check"] = "rbxassetid://86651948439229",
        ["monitor-cloud"] = "rbxassetid://85931096038318",
        ["monitor-cog"] = "rbxassetid://94345128715799",
        ["monitor-dot"] = "rbxassetid://130394010063680",
        ["monitor-down"] = "rbxassetid://97466933743423",
        ["monitor-off"] = "rbxassetid://74395526657953",
        ["monitor-pause"] = "rbxassetid://76002184067562",
        ["monitor-play"] = "rbxassetid://133018824306217",
        ["monitor-smartphone"] = "rbxassetid://84335680433378",
        ["monitor-speaker"] = "rbxassetid://81744810060380",
        ["monitor-stop"] = "rbxassetid://98708958984757",
        ["monitor-up"] = "rbxassetid://96035360858377",
        ["monitor-x"] = "rbxassetid://126265210441423",
        ["monitor"] = "rbxassetid://72664649203050",
        ["moon-star"] = "rbxassetid://82782200506348",
        ["moon"] = "rbxassetid://83380517901735",
        ["motorbike"] = "rbxassetid://94580787368233",
        ["mountain-snow"] = "rbxassetid://105315495740588",
        ["mountain"] = "rbxassetid://73269957566415",
        ["mouse-off"] = "rbxassetid://75267871697595",
        ["mouse-pointer-2-off"] = "rbxassetid://104701076865632",
        ["mouse-pointer-2"] = "rbxassetid://117093892862228",
        ["mouse-pointer-ban"] = "rbxassetid://106849413057133",
        ["mouse-pointer-click"] = "rbxassetid://107150227368485",
        ["mouse-pointer"] = "rbxassetid://72322454962935",
        ["mouse"] = "rbxassetid://73096068864710",
        ["move-3d"] = "rbxassetid://103365982054003",
        ["move-diagonal-2"] = "rbxassetid://117298577948096",
        ["move-diagonal"] = "rbxassetid://101433481954184",
        ["move-down-left"] = "rbxassetid://102819433534567",
        ["move-down-right"] = "rbxassetid://101479760041877",
        ["move-down"] = "rbxassetid://70510115135583",
        ["move-horizontal"] = "rbxassetid://88513523439149",
        ["move-left"] = "rbxassetid://137614740247980",
        ["move-right"] = "rbxassetid://132455779472989",
        ["move-up-left"] = "rbxassetid://139079815540148",
        ["move-up-right"] = "rbxassetid://105885140592646",
        ["move-up"] = "rbxassetid://84505444262658",
        ["move-vertical"] = "rbxassetid://86234730730899",
        ["move"] = "rbxassetid://116138709011735",
        ["music-2"] = "rbxassetid://134397426600888",
        ["music-3"] = "rbxassetid://94466120066498",
        ["music-4"] = "rbxassetid://132459323665838",
        ["music"] = "rbxassetid://113343203848535",
        ["navigation-2-off"] = "rbxassetid://116569611780763",
        ["navigation-2"] = "rbxassetid://81889066747907",
        ["navigation-off"] = "rbxassetid://87003270290777",
        ["navigation"] = "rbxassetid://79308213542922",
        ["network"] = "rbxassetid://127410729922644",
        ["newspaper"] = "rbxassetid://123479530460544",
        ["nfc"] = "rbxassetid://76822396542242",
        ["non-binary"] = "rbxassetid://78442360386235",
        ["notebook-pen"] = "rbxassetid://140380614761023",
        ["notebook-tabs"] = "rbxassetid://127371085570083",
        ["notebook-text"] = "rbxassetid://93061585217270",
        ["notebook"] = "rbxassetid://136132108664987",
        ["notepad-text-dashed"] = "rbxassetid://135793446376219",
        ["notepad-text"] = "rbxassetid://93404682958966",
        ["nut-off"] = "rbxassetid://78795397311573",
        ["nut"] = "rbxassetid://127146410705656",
        ["octagon-alert"] = "rbxassetid://140438367956051",
        ["octagon-minus"] = "rbxassetid://74720436795421",
        ["octagon-pause"] = "rbxassetid://103161463909039",
        ["octagon-x"] = "rbxassetid://90498161006311",
        ["octagon"] = "rbxassetid://120803515514852",
        ["omega"] = "rbxassetid://70414080018786",
        ["option"] = "rbxassetid://100776883894054",
        ["orbit"] = "rbxassetid://108926136860562",
        ["origami"] = "rbxassetid://136020626667101",
        ["package-2"] = "rbxassetid://70394974762575",
        ["package-check"] = "rbxassetid://102374216055130",
        ["package-minus"] = "rbxassetid://114492858789692",
        ["package-open"] = "rbxassetid://132890233237818",
        ["package-plus"] = "rbxassetid://129261988138366",
        ["package-search"] = "rbxassetid://95465120894145",
        ["package-x"] = "rbxassetid://70818501607442",
        ["package"] = "rbxassetid://97261141732706",
        ["paint-bucket"] = "rbxassetid://124275586663284",
        ["paint-roller"] = "rbxassetid://115248074358348",
        ["paintbrush-vertical"] = "rbxassetid://105151296591292",
        ["paintbrush"] = "rbxassetid://125572663700289",
        ["palette"] = "rbxassetid://86350350950064",
        ["panda"] = "rbxassetid://132509022802512",
        ["panel-bottom-close"] = "rbxassetid://74287004071159",
        ["panel-bottom-dashed"] = "rbxassetid://131084651621603",
        ["panel-bottom-open"] = "rbxassetid://107768659586540",
        ["panel-bottom"] = "rbxassetid://132127145048511",
        ["panel-left-close"] = "rbxassetid://126579818823552",
        ["panel-left-dashed"] = "rbxassetid://75536606374585",
        ["panel-left-open"] = "rbxassetid://111075816195767",
        ["panel-left-right-dashed"] = "rbxassetid://110100707973959",
        ["panel-left"] = "rbxassetid://97419752870313",
        ["panel-right-close"] = "rbxassetid://139528655524132",
        ["panel-right-dashed"] = "rbxassetid://94959793877311",
        ["panel-right-open"] = "rbxassetid://118114419142794",
        ["panel-right"] = "rbxassetid://116365035443156",
        ["panel-top-bottom-dashed"] = "rbxassetid://134737235653344",
        ["panel-top-close"] = "rbxassetid://83578325777808",
        ["panel-top-dashed"] = "rbxassetid://70522913169237",
        ["panel-top-open"] = "rbxassetid://137959875507454",
        ["panel-top"] = "rbxassetid://75838479462875",
        ["panels-left-bottom"] = "rbxassetid://72996856149149",
        ["panels-right-bottom"] = "rbxassetid://90659068960726",
        ["panels-top-left"] = "rbxassetid://79858853850600",
        ["paperclip"] = "rbxassetid://92088291163453",
        ["parentheses"] = "rbxassetid://78950955173096",
        ["parking-meter"] = "rbxassetid://84652733960568",
        ["party-popper"] = "rbxassetid://111626795712193",
        ["pause"] = "rbxassetid://74873705394436",
        ["paw-print"] = "rbxassetid://112218825427601",
        ["pc-case"] = "rbxassetid://122978648019101",
        ["pen-line"] = "rbxassetid://109108135755303",
        ["pen-off"] = "rbxassetid://84807123119438",
        ["pen-tool"] = "rbxassetid://106145404953445",
        ["pen"] = "rbxassetid://72037878096321",
        ["pencil-line"] = "rbxassetid://88392917053533",
        ["pencil-off"] = "rbxassetid://103330927652832",
        ["pencil-ruler"] = "rbxassetid://110120288284597",
        ["pencil"] = "rbxassetid://137986121120732",
        ["pentagon"] = "rbxassetid://79184802179890",
        ["percent"] = "rbxassetid://130155041032013",
        ["person-standing"] = "rbxassetid://125020872044147",
        ["philippine-peso"] = "rbxassetid://91173798254675",
        ["phone-call"] = "rbxassetid://70555587592860",
        ["phone-forwarded"] = "rbxassetid://113269614319737",
        ["phone-incoming"] = "rbxassetid://82863576359288",
        ["phone-missed"] = "rbxassetid://130156165198376",
        ["phone-off"] = "rbxassetid://133318623553383",
        ["phone-outgoing"] = "rbxassetid://104576478735825",
        ["phone"] = "rbxassetid://128804946640049",
        ["pi"] = "rbxassetid://74936036243146",
        ["piano"] = "rbxassetid://85008880789520",
        ["pickaxe"] = "rbxassetid://105888023317688",
        ["picture-in-picture-2"] = "rbxassetid://112803319544468",
        ["picture-in-picture"] = "rbxassetid://80579597835123",
        ["piggy-bank"] = "rbxassetid://79498575790721",
        ["pilcrow-left"] = "rbxassetid://103803000849583",
        ["pilcrow-right"] = "rbxassetid://104881733911870",
        ["pilcrow"] = "rbxassetid://139512780392871",
        ["pill-bottle"] = "rbxassetid://118394692404597",
        ["pill"] = "rbxassetid://73280534813448",
        ["pin-off"] = "rbxassetid://127696372451750",
        ["pin"] = "rbxassetid://120978111007514",
        ["pipette"] = "rbxassetid://133167932934404",
        ["pizza"] = "rbxassetid://126964453193501",
        ["plane-landing"] = "rbxassetid://122555692211889",
        ["plane-takeoff"] = "rbxassetid://117179478829575",
        ["plane"] = "rbxassetid://126985561580989",
        ["play"] = "rbxassetid://135609604299893",
        ["plug-2"] = "rbxassetid://97912386476366",
        ["plug-zap"] = "rbxassetid://74506269884055",
        ["plug"] = "rbxassetid://99782373064495",
        ["plus"] = "rbxassetid://111774323017047",
        ["pocket-knife"] = "rbxassetid://134075428063965",
        ["pocket"] = "rbxassetid://136686762542964",
        ["podcast"] = "rbxassetid://109577075549215",
        ["pointer-off"] = "rbxassetid://95488389312794",
        ["pointer"] = "rbxassetid://92615117311099",
        ["popcorn"] = "rbxassetid://139446511232750",
        ["popsicle"] = "rbxassetid://112696318077073",
        ["pound-sterling"] = "rbxassetid://127482649469130",
        ["power-off"] = "rbxassetid://118768311012214",
        ["power"] = "rbxassetid://96479131758775",
        ["presentation"] = "rbxassetid://106134583757890",
        ["printer-check"] = "rbxassetid://130273549443689",
        ["printer"] = "rbxassetid://76080649734247",
        ["projector"] = "rbxassetid://103281856385283",
        ["proportions"] = "rbxassetid://130046855997237",
        ["puzzle"] = "rbxassetid://136837798892463",
        ["pyramid"] = "rbxassetid://107811442374127",
        ["qr-code"] = "rbxassetid://105329945723350",
        ["quote"] = "rbxassetid://103271711590001",
        ["rabbit"] = "rbxassetid://98580518804206",
        ["radar"] = "rbxassetid://138528222906635",
        ["radiation"] = "rbxassetid://104499586848433",
        ["radical"] = "rbxassetid://132758286926047",
        ["radio-receiver"] = "rbxassetid://129598303378835",
        ["radio-tower"] = "rbxassetid://93958663130054",
        ["radio"] = "rbxassetid://85611589536956",
        ["radius"] = "rbxassetid://89814505307129",
        ["rail-symbol"] = "rbxassetid://134295386306962",
        ["rainbow"] = "rbxassetid://132488862841895",
        ["rat"] = "rbxassetid://127400975953159",
        ["ratio"] = "rbxassetid://126369423897295",
        ["receipt-cent"] = "rbxassetid://91557573925201",
        ["receipt-euro"] = "rbxassetid://94015722210295",
        ["receipt-indian-rupee"] = "rbxassetid://89718170439990",
        ["receipt-japanese-yen"] = "rbxassetid://132472560758851",
        ["receipt-pound-sterling"] = "rbxassetid://73934967569625",
        ["receipt-russian-ruble"] = "rbxassetid://105164576936853",
        ["receipt-swiss-franc"] = "rbxassetid://72503668620116",
        ["receipt-text"] = "rbxassetid://138483536013737",
        ["receipt-turkish-lira"] = "rbxassetid://91950765836342",
        ["receipt"] = "rbxassetid://77877895901792",
        ["rectangle-circle"] = "rbxassetid://100642423153903",
        ["rectangle-ellipsis"] = "rbxassetid://112919953980965",
        ["rectangle-goggles"] = "rbxassetid://98605436666727",
        ["rectangle-horizontal"] = "rbxassetid://90224199814966",
        ["rectangle-vertical"] = "rbxassetid://117277050590967",
        ["recycle"] = "rbxassetid://140417023381961",
        ["redo-2"] = "rbxassetid://70451039017914",
        ["redo-dot"] = "rbxassetid://94252981719732",
        ["redo"] = "rbxassetid://116150342119054",
        ["refresh-ccw-dot"] = "rbxassetid://106702246753270",
        ["refresh-ccw"] = "rbxassetid://117913330389477",
        ["refresh-cw-off"] = "rbxassetid://140179498843054",
        ["refresh-cw"] = "rbxassetid://138133190015277",
        ["refrigerator"] = "rbxassetid://102614042652753",
        ["regex"] = "rbxassetid://100727200791841",
        ["remove-formatting"] = "rbxassetid://112833162022628",
        ["repeat-1"] = "rbxassetid://130144534857095",
        ["repeat-2"] = "rbxassetid://85927537182704",
        ["repeat"] = "rbxassetid://121886242955173",
        ["replace-all"] = "rbxassetid://127862728198635",
        ["replace"] = "rbxassetid://128404082279430",
        ["reply-all"] = "rbxassetid://71723137343562",
        ["reply"] = "rbxassetid://109788633497028",
        ["rewind"] = "rbxassetid://95205297521988",
        ["ribbon"] = "rbxassetid://94265331526851",
        ["rocket"] = "rbxassetid://87412317685854",
        ["rocking-chair"] = "rbxassetid://110420269495360",
        ["roller-coaster"] = "rbxassetid://112426178972099",
        ["rose"] = "rbxassetid://126336840238769",
        ["rotate-3d"] = "rbxassetid://76300551576392",
        ["rotate-ccw-key"] = "rbxassetid://74976035240976",
        ["rotate-ccw-square"] = "rbxassetid://90515853170424",
        ["rotate-ccw"] = "rbxassetid://110116685948665",
        ["rotate-cw-square"] = "rbxassetid://77095448159303",
        ["rotate-cw"] = "rbxassetid://84183336178654",
        ["route-off"] = "rbxassetid://106350402024079",
        ["route"] = "rbxassetid://89968303228953",
        ["router"] = "rbxassetid://102130331994471",
        ["rows-2"] = "rbxassetid://112556185960101",
        ["rows-3"] = "rbxassetid://117215586961375",
        ["rows-4"] = "rbxassetid://125646021959055",
        ["rss"] = "rbxassetid://131789058984793",
        ["ruler-dimension-line"] = "rbxassetid://70673861371412",
        ["ruler"] = "rbxassetid://81432445547423",
        ["russian-ruble"] = "rbxassetid://126357936542156",
        ["sailboat"] = "rbxassetid://87110567187540",
        ["salad"] = "rbxassetid://128864507821603",
        ["sandwich"] = "rbxassetid://104573187458917",
        ["satellite-dish"] = "rbxassetid://136742443888305",
        ["satellite"] = "rbxassetid://134967053164645",
        ["saudi-riyal"] = "rbxassetid://102282769104635",
        ["save-all"] = "rbxassetid://116946975799440",
        ["save-off"] = "rbxassetid://87085435778560",
        ["save"] = "rbxassetid://126116963775616",
        ["scale-3d"] = "rbxassetid://72414199620352",
        ["scale"] = "rbxassetid://108203682317477",
        ["scaling"] = "rbxassetid://122360365318466",
        ["scan-barcode"] = "rbxassetid://96889457154761",
        ["scan-eye"] = "rbxassetid://99244790601968",
        ["scan-face"] = "rbxassetid://109959345069668",
        ["scan-heart"] = "rbxassetid://106280819776142",
        ["scan-line"] = "rbxassetid://126544908146540",
        ["scan-qr-code"] = "rbxassetid://105409149549927",
        ["scan-search"] = "rbxassetid://80009010551347",
        ["scan-text"] = "rbxassetid://73702396787766",
        ["scan"] = "rbxassetid://123104789658180",
        ["school"] = "rbxassetid://76351530290068",
        ["scissors-line-dashed"] = "rbxassetid://122237447974173",
        ["scissors"] = "rbxassetid://118665510911274",
        ["screen-share-off"] = "rbxassetid://107677572669805",
        ["screen-share"] = "rbxassetid://85137895705653",
        ["scroll-text"] = "rbxassetid://97321022666868",
        ["scroll"] = "rbxassetid://74072101474951",
        ["search-check"] = "rbxassetid://75442076191356",
        ["search-code"] = "rbxassetid://117114794592802",
        ["search-slash"] = "rbxassetid://96483932261041",
        ["search-x"] = "rbxassetid://137319957522951",
        ["search"] = "rbxassetid://121018724060431",
        ["section"] = "rbxassetid://91732188298948",
        ["send-horizontal"] = "rbxassetid://111734392411664",
        ["send-to-back"] = "rbxassetid://75340312862253",
        ["send"] = "rbxassetid://127751956873796",
        ["separator-horizontal"] = "rbxassetid://84864453699927",
        ["separator-vertical"] = "rbxassetid://84031801478581",
        ["server-cog"] = "rbxassetid://138470287250966",
        ["server-crash"] = "rbxassetid://132810618000212",
        ["server-off"] = "rbxassetid://114048751507723",
        ["server"] = "rbxassetid://92188766517878",
        ["settings-2"] = "rbxassetid://135684703553372",
        ["settings"] = "rbxassetid://80758916183665",
        ["shapes"] = "rbxassetid://129989433311409",
        ["share-2"] = "rbxassetid://71210767962065",
        ["share"] = "rbxassetid://87340985053299",
        ["sheet"] = "rbxassetid://134902122480171",
        ["shell"] = "rbxassetid://140212943563599",
        ["shield-alert"] = "rbxassetid://114995877719925",
        ["shield-ban"] = "rbxassetid://108765041044649",
        ["shield-check"] = "rbxassetid://87354736164608",
        ["shield-ellipsis"] = "rbxassetid://114794739892123",
        ["shield-half"] = "rbxassetid://117842634172647",
        ["shield-minus"] = "rbxassetid://89965059528921",
        ["shield-off"] = "rbxassetid://133426959132690",
        ["shield-plus"] = "rbxassetid://100664857995498",
        ["shield-question-mark"] = "rbxassetid://135722075265150",
        ["shield-user"] = "rbxassetid://124832775645347",
        ["shield-x"] = "rbxassetid://73370117343811",
        ["shield"] = "rbxassetid://110987169760162",
        ["ship-wheel"] = "rbxassetid://130797795829448",
        ["ship"] = "rbxassetid://83995100553930",
        ["shirt"] = "rbxassetid://106579555405966",
        ["shopping-bag"] = "rbxassetid://71885477293226",
        ["shopping-basket"] = "rbxassetid://138646411956433",
        ["shopping-cart"] = "rbxassetid://128420521375441",
        ["shovel"] = "rbxassetid://102465000512056",
        ["shower-head"] = "rbxassetid://75884944024117",
        ["shredder"] = "rbxassetid://122125164414463",
        ["shrimp"] = "rbxassetid://102625900815307",
        ["shrink"] = "rbxassetid://90953687918880",
        ["shrub"] = "rbxassetid://127326280714343",
        ["shuffle"] = "rbxassetid://132382786975101",
        ["sigma"] = "rbxassetid://126884244870899",
        ["signal-high"] = "rbxassetid://130436670012270",
        ["signal-low"] = "rbxassetid://73674683500458",
        ["signal-medium"] = "rbxassetid://125003021367019",
        ["signal-zero"] = "rbxassetid://130045332414754",
        ["signal"] = "rbxassetid://78424889355261",
        ["signature"] = "rbxassetid://114402748013000",
        ["signpost-big"] = "rbxassetid://115780185675001",
        ["signpost"] = "rbxassetid://106584743791433",
        ["siren"] = "rbxassetid://134210267818039",
        ["skip-back"] = "rbxassetid://70466132711334",
        ["skip-forward"] = "rbxassetid://124844823753990",
        ["skull"] = "rbxassetid://137726256442333",
        ["slack"] = "rbxassetid://96089719516736",
        ["slash"] = "rbxassetid://117792185664263",
        ["slice"] = "rbxassetid://95810504278179",
        ["sliders-horizontal"] = "rbxassetid://85538382643347",
        ["sliders-vertical"] = "rbxassetid://101190569086853",
        ["smartphone-charging"] = "rbxassetid://102837532613995",
        ["smartphone-nfc"] = "rbxassetid://82326425754446",
        ["smartphone"] = "rbxassetid://96623008834511",
        ["smile-plus"] = "rbxassetid://131981881472144",
        ["smile"] = "rbxassetid://105880397565283",
        ["snail"] = "rbxassetid://70904536548363",
        ["snowflake"] = "rbxassetid://101235206534566",
        ["soap-dispenser-droplet"] = "rbxassetid://77258480479465",
        ["sofa"] = "rbxassetid://114427687218324",
        ["solar-panel"] = "rbxassetid://132448188047921",
        ["soup"] = "rbxassetid://115092551871618",
        ["space"] = "rbxassetid://87072088914178",
        ["spade"] = "rbxassetid://131444449466462",
        ["sparkle"] = "rbxassetid://111044800239623",
        ["sparkles"] = "rbxassetid://138635884129147",
        ["speaker"] = "rbxassetid://96227183003618",
        ["speech"] = "rbxassetid://87013139446349",
        ["spell-check-2"] = "rbxassetid://81556731785534",
        ["spell-check"] = "rbxassetid://91913483031334",
        ["spline-pointer"] = "rbxassetid://84842840956804",
        ["spline"] = "rbxassetid://129406685807412",
        ["split"] = "rbxassetid://105112438805988",
        ["spool"] = "rbxassetid://124541981347743",
        ["spotlight"] = "rbxassetid://77571742539344",
        ["spray-can"] = "rbxassetid://128372039366326",
        ["sprout"] = "rbxassetid://100091687832508",
        ["square-activity"] = "rbxassetid://89496630185293",
        ["square-arrow-down-left"] = "rbxassetid://108194680296901",
        ["square-arrow-down-right"] = "rbxassetid://99403846801050",
        ["square-arrow-down"] = "rbxassetid://135962519626588",
        ["square-arrow-left"] = "rbxassetid://111671474549238",
        ["square-arrow-out-down-left"] = "rbxassetid://125714881756353",
        ["square-arrow-out-down-right"] = "rbxassetid://89971003001390",
        ["square-arrow-out-up-left"] = "rbxassetid://103759986579087",
        ["square-arrow-out-up-right"] = "rbxassetid://91221896066807",
        ["square-arrow-right"] = "rbxassetid://113920471701361",
        ["square-arrow-up-left"] = "rbxassetid://112424670290693",
        ["square-arrow-up-right"] = "rbxassetid://76602291406940",
        ["square-arrow-up"] = "rbxassetid://106998604646718",
        ["square-asterisk"] = "rbxassetid://89186832353625",
        ["square-bottom-dashed-scissors"] = "rbxassetid://79076980104803",
        ["square-chart-gantt"] = "rbxassetid://104034017316411",
        ["square-check-big"] = "rbxassetid://115320390907184",
        ["square-check"] = "rbxassetid://134682053539509",
        ["square-chevron-down"] = "rbxassetid://91032307924592",
        ["square-chevron-left"] = "rbxassetid://73143404829510",
        ["square-chevron-right"] = "rbxassetid://90612077729930",
        ["square-chevron-up"] = "rbxassetid://85565910197337",
        ["square-code"] = "rbxassetid://81604576616881",
        ["square-dashed-bottom-code"] = "rbxassetid://100354801563230",
        ["square-dashed-bottom"] = "rbxassetid://101102319625624",
        ["square-dashed-kanban"] = "rbxassetid://90388067649847",
        ["square-dashed-mouse-pointer"] = "rbxassetid://121016142178467",
        ["square-dashed-top-solid"] = "rbxassetid://117157577548540",
        ["square-dashed"] = "rbxassetid://136905537847606",
        ["square-divide"] = "rbxassetid://99894657101970",
        ["square-dot"] = "rbxassetid://116613421354866",
        ["square-equal"] = "rbxassetid://110283363706707",
        ["square-function"] = "rbxassetid://86075219551088",
        ["square-kanban"] = "rbxassetid://114537101260131",
        ["square-library"] = "rbxassetid://73810931222081",
        ["square-m"] = "rbxassetid://117662700410577",
        ["square-menu"] = "rbxassetid://104067089444415",
        ["square-minus"] = "rbxassetid://116764432015770",
        ["square-mouse-pointer"] = "rbxassetid://76141850603920",
        ["square-parking-off"] = "rbxassetid://100857293535141",
        ["square-parking"] = "rbxassetid://133116656122387",
        ["square-pause"] = "rbxassetid://86608552787615",
        ["square-pen"] = "rbxassetid://120239476110475",
        ["square-percent"] = "rbxassetid://87111930314567",
        ["square-pi"] = "rbxassetid://75383328781618",
        ["square-pilcrow"] = "rbxassetid://131854284699367",
        ["square-play"] = "rbxassetid://108186325238481",
        ["square-plus"] = "rbxassetid://114713264461873",
        ["square-power"] = "rbxassetid://129240437805187",
        ["square-radical"] = "rbxassetid://132645931868292",
        ["square-round-corner"] = "rbxassetid://104592745113567",
        ["square-scissors"] = "rbxassetid://110601255612411",
        ["square-sigma"] = "rbxassetid://113231244246816",
        ["square-slash"] = "rbxassetid://105477013908757",
        ["square-split-horizontal"] = "rbxassetid://76095370148660",
        ["square-split-vertical"] = "rbxassetid://88589192032058",
        ["square-square"] = "rbxassetid://136555087357875",
        ["square-stack"] = "rbxassetid://100463396619394",
        ["square-star"] = "rbxassetid://94506958703720",
        ["square-stop"] = "rbxassetid://80018708472943",
        ["square-terminal"] = "rbxassetid://83969264476798",
        ["square-user-round"] = "rbxassetid://86484997229302",
        ["square-user"] = "rbxassetid://70771214183445",
        ["square-x"] = "rbxassetid://125136183850190",
        ["square"] = "rbxassetid://86304921356806",
        ["squares-exclude"] = "rbxassetid://102345385822324",
        ["squares-intersect"] = "rbxassetid://120869602570119",
        ["squares-subtract"] = "rbxassetid://131484650948795",
        ["squares-unite"] = "rbxassetid://96673080107843",
        ["squircle-dashed"] = "rbxassetid://129936702532522",
        ["squircle"] = "rbxassetid://82426632573807",
        ["squirrel"] = "rbxassetid://112864252085343",
        ["stamp"] = "rbxassetid://92370779813368",
        ["star-half"] = "rbxassetid://117449275562979",
        ["star-off"] = "rbxassetid://75742832732503",
        ["star"] = "rbxassetid://136141469398409",
        ["step-back"] = "rbxassetid://108672750005121",
        ["step-forward"] = "rbxassetid://126131872136145",
        ["stethoscope"] = "rbxassetid://122331031702148",
        ["sticker"] = "rbxassetid://79938203791608",
        ["sticky-note"] = "rbxassetid://111894074643919",
        ["store"] = "rbxassetid://90338129673705",
        ["stretch-horizontal"] = "rbxassetid://87665042192343",
        ["stretch-vertical"] = "rbxassetid://95265463417122",
        ["strikethrough"] = "rbxassetid://103417324549613",
        ["subscript"] = "rbxassetid://74553514785183",
        ["sun-dim"] = "rbxassetid://129141645592715",
        ["sun-medium"] = "rbxassetid://130278807964710",
        ["sun-moon"] = "rbxassetid://75752898854559",
        ["sun-snow"] = "rbxassetid://112791898014579",
        ["sun"] = "rbxassetid://110150589884127",
        ["sunrise"] = "rbxassetid://134705665494098",
        ["sunset"] = "rbxassetid://75904872203588",
        ["superscript"] = "rbxassetid://96887696590118",
        ["swatch-book"] = "rbxassetid://126786244872453",
        ["swiss-franc"] = "rbxassetid://113497920041625",
        ["switch-camera"] = "rbxassetid://76841154349737",
        ["sword"] = "rbxassetid://124448418211665",
        ["swords"] = "rbxassetid://81872698913435",
        ["syringe"] = "rbxassetid://123891270479254",
        ["table-2"] = "rbxassetid://95751552281545",
        ["table-cells-merge"] = "rbxassetid://95363715175258",
        ["table-cells-split"] = "rbxassetid://114799086088649",
        ["table-columns-split"] = "rbxassetid://111011625447949",
        ["table-of-contents"] = "rbxassetid://135044763275414",
        ["table-properties"] = "rbxassetid://125062886015372",
        ["table-rows-split"] = "rbxassetid://96443733673997",
        ["table"] = "rbxassetid://109109148250737",
        ["tablet-smartphone"] = "rbxassetid://133680859813404",
        ["tablet"] = "rbxassetid://128403991264386",
        ["tablets"] = "rbxassetid://80835787970735",
        ["tag"] = "rbxassetid://129104970103940",
        ["tags"] = "rbxassetid://107179263080798",
        ["tally-1"] = "rbxassetid://115301298241643",
        ["tally-2"] = "rbxassetid://110363186864027",
        ["tally-3"] = "rbxassetid://97655344572540",
        ["tally-4"] = "rbxassetid://102633494371890",
        ["tally-5"] = "rbxassetid://88031817475886",
        ["tangent"] = "rbxassetid://123263132981724",
        ["target"] = "rbxassetid://87563802520297",
        ["telescope"] = "rbxassetid://91755049143647",
        ["tent-tree"] = "rbxassetid://76698322463977",
        ["tent"] = "rbxassetid://109779587826330",
        ["terminal"] = "rbxassetid://106783148545356",
        ["test-tube-diagonal"] = "rbxassetid://75662704378840",
        ["test-tube"] = "rbxassetid://98801015650164",
        ["test-tubes"] = "rbxassetid://92555361447433",
        ["text-align-center"] = "rbxassetid://84051028246390",
        ["text-align-end"] = "rbxassetid://130041738343555",
        ["text-align-justify"] = "rbxassetid://80279880143030",
        ["text-align-start"] = "rbxassetid://134489585487649",
        ["text-cursor-input"] = "rbxassetid://107551944047171",
        ["text-cursor"] = "rbxassetid://115984654447300",
        ["text-initial"] = "rbxassetid://129458097472087",
        ["text-quote"] = "rbxassetid://139278366448736",
        ["text-search"] = "rbxassetid://92345384671606",
        ["text-select"] = "rbxassetid://117087320884956",
        ["text-wrap"] = "rbxassetid://114804318314018",
        ["theater"] = "rbxassetid://108558145549163",
        ["thermometer-snowflake"] = "rbxassetid://121876188028425",
        ["thermometer-sun"] = "rbxassetid://106693240074310",
        ["thermometer"] = "rbxassetid://106546011492311",
        ["thumbs-down"] = "rbxassetid://87794009914015",
        ["thumbs-up"] = "rbxassetid://111137070767020",
        ["ticket-check"] = "rbxassetid://105428777212507",
        ["ticket-minus"] = "rbxassetid://78966299769328",
        ["ticket-percent"] = "rbxassetid://80834774406405",
        ["ticket-plus"] = "rbxassetid://110086734392189",
        ["ticket-slash"] = "rbxassetid://89045681172265",
        ["ticket-x"] = "rbxassetid://88674114109926",
        ["ticket"] = "rbxassetid://126527071492145",
        ["tickets-plane"] = "rbxassetid://100367018248695",
        ["tickets"] = "rbxassetid://135268612687833",
        ["timer-off"] = "rbxassetid://110916370767271",
        ["timer-reset"] = "rbxassetid://110052125369932",
        ["timer"] = "rbxassetid://85473888890506",
        ["toggle-left"] = "rbxassetid://85887872573050",
        ["toggle-right"] = "rbxassetid://90411952142550",
        ["toilet"] = "rbxassetid://80930782432931",
        ["tool-case"] = "rbxassetid://87533537832522",
        ["tornado"] = "rbxassetid://88358291515768",
        ["torus"] = "rbxassetid://70855707283051",
        ["touchpad-off"] = "rbxassetid://78784008075456",
        ["touchpad"] = "rbxassetid://74882354908014",
        ["tower-control"] = "rbxassetid://95937619060532",
        ["toy-brick"] = "rbxassetid://86293483924633",
        ["tractor"] = "rbxassetid://103376704722051",
        ["traffic-cone"] = "rbxassetid://74110220470369",
        ["train-front-tunnel"] = "rbxassetid://105194827005114",
        ["train-front"] = "rbxassetid://125237934215370",
        ["train-track"] = "rbxassetid://77451032453723",
        ["tram-front"] = "rbxassetid://93315182364998",
        ["transgender"] = "rbxassetid://135530817673639",
        ["trash-2"] = "rbxassetid://109843431391323",
        ["trash"] = "rbxassetid://106723740584310",
        ["tree-deciduous"] = "rbxassetid://123124389219004",
        ["tree-palm"] = "rbxassetid://103846705893963",
        ["tree-pine"] = "rbxassetid://124662547202594",
        ["trees"] = "rbxassetid://121203841375919",
        ["trello"] = "rbxassetid://130987241149527",
        ["trending-down"] = "rbxassetid://139309232226438",
        ["trending-up-down"] = "rbxassetid://85083293981691",
        ["trending-up"] = "rbxassetid://81819858538839",
        ["triangle-alert"] = "rbxassetid://125920361880643",
        ["triangle-dashed"] = "rbxassetid://124324079103935",
        ["triangle-right"] = "rbxassetid://116930791412791",
        ["triangle"] = "rbxassetid://126330486745540",
        ["trophy"] = "rbxassetid://131545003268773",
        ["truck-electric"] = "rbxassetid://111873446387359",
        ["truck"] = "rbxassetid://86662707764771",
        ["turkish-lira"] = "rbxassetid://114589876174070",
        ["turntable"] = "rbxassetid://129870346487856",
        ["turtle"] = "rbxassetid://118295081560334",
        ["tv-minimal-play"] = "rbxassetid://99201833426972",
        ["tv-minimal"] = "rbxassetid://100382201729427",
        ["tv"] = "rbxassetid://135687724791776",
        ["twitch"] = "rbxassetid://71383308134888",
        ["twitter"] = "rbxassetid://88791703276842",
        ["type-outline"] = "rbxassetid://80108627791690",
        ["type"] = "rbxassetid://133543553793564",
        ["umbrella-off"] = "rbxassetid://72395143739955",
        ["umbrella"] = "rbxassetid://127502210274589",
        ["underline"] = "rbxassetid://123709229216544",
        ["undo-2"] = "rbxassetid://113885292059932",
        ["undo-dot"] = "rbxassetid://132055277744844",
        ["undo"] = "rbxassetid://111258459077271",
        ["unfold-horizontal"] = "rbxassetid://117128358526398",
        ["unfold-vertical"] = "rbxassetid://116593025265499",
        ["ungroup"] = "rbxassetid://106674800451003",
        ["university"] = "rbxassetid://84652528263642",
        ["unlink-2"] = "rbxassetid://128131898892572",
        ["unlink"] = "rbxassetid://139835795227752",
        ["unplug"] = "rbxassetid://90171381619874",
        ["upload"] = "rbxassetid://138212042425501",
        ["usb"] = "rbxassetid://117230058949613",
        ["user-check"] = "rbxassetid://81775205032725",
        ["user-cog"] = "rbxassetid://92795491530865",
        ["user-lock"] = "rbxassetid://78892639693821",
        ["user-minus"] = "rbxassetid://126976941957511",
        ["user-pen"] = "rbxassetid://87445472574836",
        ["user-plus"] = "rbxassetid://118514469915884",
        ["user-round-check"] = "rbxassetid://118794737621941",
        ["user-round-cog"] = "rbxassetid://78239503290053",
        ["user-round-minus"] = "rbxassetid://98944176636447",
        ["user-round-pen"] = "rbxassetid://108155244324878",
        ["user-round-plus"] = "rbxassetid://113301899567470",
        ["user-round-search"] = "rbxassetid://71565774381870",
        ["user-round-x"] = "rbxassetid://122367980560930",
        ["user-round"] = "rbxassetid://136485052187963",
        ["user-search"] = "rbxassetid://101335649828115",
        ["user-star"] = "rbxassetid://98777846316000",
        ["user-x"] = "rbxassetid://139748155894754",
        ["user"] = "rbxassetid://81589895647169",
        ["users-round"] = "rbxassetid://103005444008339",
        ["users"] = "rbxassetid://115398113982385",
        ["utensils-crossed"] = "rbxassetid://109520762270383",
        ["utensils"] = "rbxassetid://139952569804235",
        ["utility-pole"] = "rbxassetid://101965541238242",
        ["variable"] = "rbxassetid://104743088438151",
        ["vault"] = "rbxassetid://108049164599845",
        ["vector-square"] = "rbxassetid://86713728565344",
        ["vegan"] = "rbxassetid://119489190688082",
        ["venetian-mask"] = "rbxassetid://102636443033920",
        ["venus-and-mars"] = "rbxassetid://120227752103771",
        ["venus"] = "rbxassetid://82891342220859",
        ["vibrate-off"] = "rbxassetid://113446447326246",
        ["vibrate"] = "rbxassetid://108330910738733",
        ["video-off"] = "rbxassetid://132239189859305",
        ["video"] = "rbxassetid://107587444636945",
        ["videotape"] = "rbxassetid://114816894323398",
        ["view"] = "rbxassetid://118717253976805",
        ["voicemail"] = "rbxassetid://134313454010227",
        ["volleyball"] = "rbxassetid://83889351124153",
        ["volume-1"] = "rbxassetid://98514588731639",
        ["volume-2"] = "rbxassetid://89344380902620",
        ["volume-off"] = "rbxassetid://103047478058767",
        ["volume-x"] = "rbxassetid://139252359189540",
        ["volume"] = "rbxassetid://103236289817396",
        ["vote"] = "rbxassetid://89409762851246",
        ["wallet-cards"] = "rbxassetid://129728715308337",
        ["wallet-minimal"] = "rbxassetid://137800448816116",
        ["wallet"] = "rbxassetid://132331555762628",
        ["wallpaper"] = "rbxassetid://74682121235494",
        ["wand-sparkles"] = "rbxassetid://82546429942392",
        ["wand"] = "rbxassetid://114580617777835",
        ["warehouse"] = "rbxassetid://78388887451080",
        ["washing-machine"] = "rbxassetid://104194127573858",
        ["watch"] = "rbxassetid://130544621618405",
        ["waves-ladder"] = "rbxassetid://101808619355514",
        ["waves"] = "rbxassetid://96340135183647",
        ["waypoints"] = "rbxassetid://102450133666017",
        ["webcam"] = "rbxassetid://104148487911129",
        ["webhook-off"] = "rbxassetid://96370548093471",
        ["webhook"] = "rbxassetid://112812457747322",
        ["weight"] = "rbxassetid://103860559844854",
        ["wheat-off"] = "rbxassetid://133294844612307",
        ["wheat"] = "rbxassetid://85261952080359",
        ["whole-word"] = "rbxassetid://90111083954485",
        ["wifi-cog"] = "rbxassetid://110500263326209",
        ["wifi-high"] = "rbxassetid://81954601342139",
        ["wifi-low"] = "rbxassetid://138217335635913",
        ["wifi-off"] = "rbxassetid://74113634330106",
        ["wifi-pen"] = "rbxassetid://91290205064712",
        ["wifi-sync"] = "rbxassetid://84043971055177",
        ["wifi-zero"] = "rbxassetid://124286465246123",
        ["wifi"] = "rbxassetid://104669375183960",
        ["wind-arrow-down"] = "rbxassetid://127753987414870",
        ["wind"] = "rbxassetid://114551690399915",
        ["wine-off"] = "rbxassetid://108294164302317",
        ["wine"] = "rbxassetid://115743721332829",
        ["workflow"] = "rbxassetid://99186544029189",
        ["worm"] = "rbxassetid://115752311548091",
        ["wrench"] = "rbxassetid://112148279212860",
        ["x"] = "rbxassetid://110786993356448",
        ["youtube"] = "rbxassetid://123663668456341",
        ["zap-off"] = "rbxassetid://81385483183652",
        ["zap"] = "rbxassetid://130551565616516",
        ["zoom-in"] = "rbxassetid://127956924984803",
        ["zoom-out"] = "rbxassetid://108334162607319",
        ["balloon"] = "rbxassetid://97489111621526",
        ["beef-off"] = "rbxassetid://99869959725200",
        ["book-search"] = "rbxassetid://132585409504950",
        ["calendars"] = "rbxassetid://130944763042289",
        ["cannabis-off"] = "rbxassetid://101938500363812",
        ["cctv-off"] = "rbxassetid://75925370187295",
        ["cigarette"] = "rbxassetid://137149549886852",
        ["circle-pile"] = "rbxassetid://116353155251541",
        ["cloud-backup"] = "rbxassetid://111649579696132",
        ["cloud-sync"] = "rbxassetid://79393911188593",
        ["database-search"] = "rbxassetid://92017137080138",
        ["ellipse"] = "rbxassetid://71559658267482",
        ["fingerprint-pattern"] = "rbxassetid://80934710831288",
        ["fishing-hook"] = "rbxassetid://121038780855899",
        ["fishing-rod"] = "rbxassetid://71754848048049",
        ["form"] = "rbxassetid://72999643971000",
        ["git-merge-conflict"] = "rbxassetid://85677801675703",
        ["globe-off"] = "rbxassetid://77775243585824",
        ["globe-x"] = "rbxassetid://109268097029296",
        ["hd"] = "rbxassetid://71682790698278",
        ["image"] = "rbxassetid://112751259236831",
        ["layers-plus"] = "rbxassetid://77587765623057",
        ["lens-concave"] = "rbxassetid://94819631937027",
        ["lens-convex"] = "rbxassetid://74736504195474",
        ["line-dot-right-horizontal"] = "rbxassetid://104718593155221",
        ["line-style"] = "rbxassetid://90176717785772",
        ["map-pin-search"] = "rbxassetid://89065012915078",
        ["message-circle-check"] = "rbxassetid://132772297689418",
        ["message-square-check"] = "rbxassetid://125789987055668",
        ["metronome"] = "rbxassetid://101991829345965",
        ["mirror-rectangular"] = "rbxassetid://109046769760336",
        ["mirror-round"] = "rbxassetid://121534049429097",
        ["mouse-left"] = "rbxassetid://99144293708743",
        ["mouse-right"] = "rbxassetid://88331710212594",
        ["printer-x"] = "rbxassetid://103002721801548",
        ["radio-off"] = "rbxassetid://80359258046586",
        ["road"] = "rbxassetid://120251329173530",
        ["scooter"] = "rbxassetid://100035452787934",
        ["search-alert"] = "rbxassetid://127597984617505",
        ["shelving-unit"] = "rbxassetid://80116568514793",
        ["shield-cog-corner"] = "rbxassetid://111694066132698",
        ["shield-cog"] = "rbxassetid://129235695057857",
        ["sport-shoe"] = "rbxassetid://120495992692630",
        ["square-arrow-right-enter"] = "rbxassetid://138867831495334",
        ["square-arrow-right-exit"] = "rbxassetid://133688575845430",
        ["square-centerline-dashed-horizontal"] = "rbxassetid://77780104374341",
        ["square-centerline-dashed-vertical"] = "rbxassetid://107878435803525",
        ["stone"] = "rbxassetid://135161057497830",
        ["toolbox"] = "rbxassetid://85341033903792",
        ["towel-rack"] = "rbxassetid://125223915620991",
        ["user-key"] = "rbxassetid://105403041782190",
        ["user-round-key"] = "rbxassetid://124547549008939",
        ["van"] = "rbxassetid://122066377022942",
        ["waves-arrow-down"] = "rbxassetid://129215220911792",
        ["waves-arrow-up"] = "rbxassetid://102314705716217",
        ["weight-tilde"] = "rbxassetid://112081212176951",
        ["x-line-top"] = "rbxassetid://140592656289509",
        ["zodiac-aquarius"] = "rbxassetid://74560047770362",
        ["zodiac-aries"] = "rbxassetid://73255859670234",
        ["zodiac-cancer"] = "rbxassetid://131985162532947",
        ["zodiac-capricorn"] = "rbxassetid://97859568140652",
        ["zodiac-gemini"] = "rbxassetid://80997588122992",
        ["zodiac-leo"] = "rbxassetid://75509406718106",
        ["zodiac-libra"] = "rbxassetid://113222735060218",
        ["zodiac-ophiuchus"] = "rbxassetid://129180108892480",
        ["zodiac-pisces"] = "rbxassetid://95845819440327",
        ["zodiac-sagittarius"] = "rbxassetid://82651026742181",
        ["zodiac-scorpio"] = "rbxassetid://113640924054631",
        ["zodiac-taurus"] = "rbxassetid://123053219704400",
        ["zodiac-virgo"] = "rbxassetid://99462994613661",
    }
    local Aliases = {
        ["home"] = "house",
        ["home-icon"] = "house",
        ["sliders"] = "sliders-horizontal",
        ["edit"] = "square-pen",
        ["edit-2"] = "pen",
        ["edit-3"] = "pen-line",
        ["unlock"] = "lock-open",
        ["unlock-keyhole"] = "lock-keyhole-open",
        ["grid"] = "layout-grid",
        ["bar-chart"] = "chart-column",
        ["bar-chart-2"] = "chart-column",
        ["bar-chart-3"] = "chart-column",
        ["bar-chart-4"] = "chart-bar",
        ["bar-chart-big"] = "chart-column-big",
        ["pie-chart"] = "chart-pie",
        ["line-chart"] = "chart-line",
        ["area-chart"] = "chart-area",
        ["candlestick-chart"] = "chart-candlestick",
        ["scatter-chart"] = "chart-scatter",
        ["gantt-chart"] = "chart-gantt",
        ["alert-triangle"] = "triangle-alert",
        ["alert-circle"] = "circle-alert",
        ["alert-octagon"] = "octagon-alert",
        ["check-circle"] = "circle-check",
        ["check-circle-2"] = "circle-check",
        ["check-square"] = "square-check",
        ["check-square-2"] = "square-check",
        ["x-circle"] = "circle-x",
        ["x-octagon"] = "octagon-x",
        ["x-square"] = "square-x",
        ["plus-circle"] = "circle-plus",
        ["plus-square"] = "square-plus",
        ["minus-circle"] = "circle-minus",
        ["minus-square"] = "square-minus",
        ["divide-circle"] = "circle-divide",
        ["divide-square"] = "square-divide",
        ["percent-circle"] = "circle-percent",
        ["percent-square"] = "square-percent",
        ["help-circle"] = "circle-question-mark",
        ["circle-help"] = "circle-question-mark",
        ["badge-help"] = "badge-question-mark",
        ["circle-info"] = "info",
        ["more-horizontal"] = "ellipsis",
        ["more-vertical"] = "ellipsis-vertical",
        ["loader-2"] = "loader-circle",
        ["arrow-up-circle"] = "circle-arrow-up",
        ["arrow-down-circle"] = "circle-arrow-down",
        ["arrow-left-circle"] = "circle-arrow-left",
        ["arrow-right-circle"] = "circle-arrow-right",
        ["chevron-up-circle"] = "circle-chevron-up",
        ["chevron-down-circle"] = "circle-chevron-down",
        ["chevron-left-circle"] = "circle-chevron-left",
        ["chevron-right-circle"] = "circle-chevron-right",
        ["play-circle"] = "circle-play",
        ["pause-circle"] = "circle-pause",
        ["stop-circle"] = "circle-stop",
        ["user-circle"] = "circle-user",
        ["user-circle-2"] = "circle-user-round",
        ["user-2"] = "user-round",
        ["users-2"] = "users-round",
        ["user-check-2"] = "user-round-check",
        ["user-cog-2"] = "user-round-cog",
        ["user-minus-2"] = "user-round-minus",
        ["user-plus-2"] = "user-round-plus",
        ["user-x-2"] = "user-round-x",
        ["contact-2"] = "contact-round",
        ["globe-2"] = "earth",
        ["wand-2"] = "wand-sparkles",
        ["laptop-2"] = "laptop-minimal",
        ["tv-2"] = "tv-minimal",
        ["wallet-2"] = "wallet-minimal",
        ["tool"] = "wrench",
        ["tools"] = "wrench",
        ["gear"] = "settings",
        ["discord"] = "message-circle",
        ["combat"] = "swords",
        ["pvp"] = "swords",
        ["farm"] = "sword",
        ["autofarm"] = "sword",
        ["auto-farm"] = "sword",
        ["teleport"] = "map-pin",
        ["esp"] = "scan-eye",
        ["visual"] = "eye",
        ["visuals"] = "eye",
        ["player"] = "user",
        ["players"] = "users",
        ["shop"] = "shopping-cart",
        ["misc"] = "wrench",
        ["config"] = "sliders-horizontal",
    }
    local AutoTabRules = {
        { icon = "webhook", keywords = { "webhook", "webhooks" } },
        { icon = "message-circle", keywords = { "discord", "community", "chat", "social" } },
        { icon = "bell", keywords = { "notify", "notification", "notifications", "alert", "alerts", "thong bao", "thông báo" } },
        { icon = "fish", keywords = { "fish", "fishing", "rod", "reel", "angler", "cau ca", "câu cá" } },
        { icon = "pickaxe", keywords = { "mine", "mining", "ore", "ores", "dig", "digging", "dao khoang", "đào" } },
        { icon = "sprout", keywords = { "garden", "plant", "plants", "seed", "seeds", "crop", "crops", "harvest", "tree", "trong cay", "trồng" } },
        { icon = "anchor", keywords = { "sea", "leviathan", "mirage", "kitsune", "prehistoric", "boat", "boats", "ship", "ocean", "shark", "pirate", "bien", "su kien bien" } },
        { icon = "cherry", keywords = { "fruit", "fruits", "devil fruit", "blox fruit", "berry", "trai", "trai ac quy" } },
        { icon = "zap", keywords = { "race", "v4", "v3", "draco", "cyborg", "ghoul", "mink", "angel", "awakening", "awaken", "evolution", "evolve", "toc", "thuc tinh" } },
        { icon = "flame", keywords = { "raid", "raids", "dungeon", "dungeons", "law", "trial", "trials", "hell", "flame", "mastery", "thong thao", "thông thạo" } },
        { icon = "skull", keywords = { "boss", "bosses", "mob", "mobs", "monster", "monsters", "elite", "terror", "rip indra", "katakuri" } },
        { icon = "crosshair", keywords = { "aim", "aimbot", "silent aim", "hitbox", "hitboxes", "gun", "guns", "shoot", "sniper", "triggerbot", "fov" } },
        { icon = "swords", keywords = { "combat", "pvp", "fight", "fighting", "attack", "kill", "bounty", "hunter", "melee", "weapon", "weapons", "blade", "skill", "skills", "chien dau", "danh" } },
        { icon = "shield", keywords = { "defense", "defence", "parry", "block", "safe", "anti", "antiban", "anti ban", "bypass", "godmode", "security", "bao ve", "bảo vệ" } },
        { icon = "sword", keywords = { "farm", "farming", "autofarm", "grind", "grinding", "level", "bone", "bones", "ectoplasm", "chest", "chests", "cay", "cày" } },
        { icon = "scroll-text", keywords = { "quest", "quests", "mission", "missions", "story", "scroll", "scrolls", "puzzle", "saber", "cdk", "ttk", "soul guitar", "nhiem vu", "nhiệm vụ" } },
        { icon = "chart-column", keywords = { "stat", "stats", "status", "point", "points", "leaderboard", "rank", "analytics", "chi so", "chỉ số" } },
        { icon = "hammer", keywords = { "craft", "crafting", "forge", "forging", "enchant", "upgrade", "upgrades", "ren", "nang cap" } },
        { icon = "backpack", keywords = { "item", "items", "inventory", "backpack", "bag", "material", "materials", "accessory", "accessories", "loadout", "gear", "vat pham", "kho do", "tui do" } },
        { icon = "paw-print", keywords = { "pet", "pets", "egg", "eggs", "hatch", "hatching", "mount", "mounts", "dragon", "thu cung", "thú cưng" } },
        { icon = "dices", keywords = { "gacha", "spin", "spins", "roll", "rolls", "random", "luck", "lucky", "casino", "quay" } },
        { icon = "shopping-cart", keywords = { "shop", "shops", "store", "buy", "purchase", "merchant", "dealer", "trade", "trading", "market", "cua hang", "cửa hàng", "mua" } },
        { icon = "scan-eye", keywords = { "esp", "wallhack", "chams", "tracers", "radar" } },
        { icon = "eye", keywords = { "visual", "visuals", "render", "camera", "fov", "shader", "lighting", "bright", "fullbright", "hien thi", "hiển thị" } },
        { icon = "map-pin", keywords = { "teleport", "teleports", "tp", "travel", "island", "islands", "world", "zone", "zones", "location", "locations", "map", "waypoint", "dich chuyen", "dao" } },
        { icon = "compass", keywords = { "compass", "navigate", "navigation", "find", "finder", "tracker", "locate" } },
        { icon = "users", keywords = { "players", "team", "teams", "crew", "party", "friends", "allies", "clan" } },
        { icon = "user", keywords = { "player", "localplayer", "character", "movement", "walkspeed", "jumppower", "fly", "noclip", "avatar", "profile", "nguoi choi", "nhan vat" } },
        { icon = "server", keywords = { "server", "servers", "hop", "serverhop", "rejoin", "jobid", "region", "may chu", "máy chủ" } },
        { icon = "terminal", keywords = { "script", "scripts", "executor", "console", "log", "logs", "debug", "command", "commands", "cmd" } },
        { icon = "key-round", keywords = { "key", "keys", "keybind", "keybinds", "hotkey", "hotkeys", "auth", "license" } },
        { icon = "gift", keywords = { "event", "events", "gift", "gifts", "reward", "rewards", "redeem", "code", "codes", "christmas", "halloween", "valentine", "su kien", "qua" } },
        { icon = "bot", keywords = { "bot", "macro", "macros", "ai", "automation", "auto", "afk" } },
        { icon = "settings", keywords = { "setting", "settings", "config", "configs", "configuration", "theme", "themes", "ui", "option", "options", "preference", "save", "cai dat", "cau hinh" } },
        { icon = "wrench", keywords = { "misc", "miscellaneous", "other", "others", "extra", "extras", "utility", "utilities", "tool", "tools", "helper", "tien ich", "tiện ích", "khac", "khác" } },
        { icon = "layout-dashboard", keywords = { "dashboard", "overview", "panel", "hub", "control" } },
        { icon = "info", keywords = { "info", "information", "about", "credit", "credits", "changelog", "update", "updates", "help", "guide", "faq", "thong tin", "gioi thieu" } },
        { icon = "house", keywords = { "home", "main", "general", "start", "welcome", "lobby", "trang chu", "chung", "chinh" } },
    }
    local remoteFetched = false
    local tryLoadRemoteIcons = function()
        if remoteFetched then
            return
        end
        remoteFetched = true
        pcall(function()
            if game and game.HttpGet then
                local src = game:HttpGet("https://raw.githubusercontent.com/Footagesus/Icons/refs/heads/main/lucide/dist/Icons.lua")
                if type(src) == "string" and #src > 0 then
                    local loader = loadstring or load
                    if loader then
                        local fn = loader(src)
                        if fn then
                            local data = fn()
                            if type(data) == "table" then
                                for k, v in pairs(data) do
                                    if type(k) == "string" and type(v) == "string" and not Icons[k] then
                                        Icons[k] = v
                                    end
                                end
                            end
                        end
                    end
                end
            end
        end)
    end
    local lookupKey = function(key)
        local direct = Icons[key]
        if direct then
            return direct
        end
        local aliasTarget = Aliases[key]
        if aliasTarget and Icons[aliasTarget] then
            return Icons[aliasTarget]
        end
        return nil
    end
    local getIcon = function(iconInput)
        if iconInput == nil or iconInput == false then
            return nil
        end
        if type(iconInput) == "number" then
            return "rbxassetid://" .. tostring(iconInput)
        end
        if type(iconInput) ~= "string" then
            return nil
        end
        local trimmed = iconInput:match("^%s*(.-)%s*$")
        if trimmed == "" or trimmed:lower() == "none" then
            return nil
        end
        if trimmed:match("^rbxassetid://") or trimmed:match("^rbxthumb://") or trimmed:match("^rbxasset://") or trimmed:match("^https?://") then
            return trimmed
        end
        if trimmed:match("^%d+$") then
            return "rbxassetid://" .. trimmed
        end
        local stripped = trimmed:gsub("^[Ll][Uu][Cc][Ii][Dd][Ee][:%-_]", "")
        local k1 = stripped:lower():gsub("[_%s]+", "-")
        local found = lookupKey(k1)
        if found then
            return found
        end
        local k2 = stripped:gsub("(%l)(%u)", "%1-%2"):lower():gsub("[_%s]+", "-")
        found = lookupKey(k2)
        if found then
            return found
        end
        local k3 = k2:gsub("(%a)(%d)", "%1-%2")
        found = lookupKey(k3)
        if found then
            return found
        end
        tryLoadRemoteIcons()
        return lookupKey(k1) or lookupKey(k2) or lookupKey(k3)
    end
    local VnFold = { ["à"] = "a", ["á"] = "a", ["ả"] = "a", ["ã"] = "a", ["ạ"] = "a", ["ă"] = "a", ["ằ"] = "a", ["ắ"] = "a", ["ẳ"] = "a", ["ẵ"] = "a", ["ặ"] = "a", ["â"] = "a", ["ầ"] = "a", ["ấ"] = "a", ["ẩ"] = "a", ["ẫ"] = "a", ["ậ"] = "a", ["À"] = "A", ["Á"] = "A", ["Ả"] = "A", ["Ã"] = "A", ["Ạ"] = "A", ["Ă"] = "A", ["Ằ"] = "A", ["Ắ"] = "A", ["Ẳ"] = "A", ["Ẵ"] = "A", ["Ặ"] = "A", ["Â"] = "A", ["Ầ"] = "A", ["Ấ"] = "A", ["Ẩ"] = "A", ["Ẫ"] = "A", ["Ậ"] = "A", ["đ"] = "d", ["Đ"] = "D", ["è"] = "e", ["é"] = "e", ["ẻ"] = "e", ["ẽ"] = "e", ["ẹ"] = "e", ["ê"] = "e", ["ề"] = "e", ["ế"] = "e", ["ể"] = "e", ["ễ"] = "e", ["ệ"] = "e", ["È"] = "E", ["É"] = "E", ["Ẻ"] = "E", ["Ẽ"] = "E", ["Ẹ"] = "E", ["Ê"] = "E", ["Ề"] = "E", ["Ế"] = "E", ["Ể"] = "E", ["Ễ"] = "E", ["Ệ"] = "E", ["ì"] = "i", ["í"] = "i", ["ỉ"] = "i", ["ĩ"] = "i", ["ị"] = "i", ["Ì"] = "I", ["Í"] = "I", ["Ỉ"] = "I", ["Ĩ"] = "I", ["Ị"] = "I", ["ò"] = "o", ["ó"] = "o", ["ỏ"] = "o", ["õ"] = "o", ["ọ"] = "o", ["ô"] = "o", ["ồ"] = "o", ["ố"] = "o", ["ổ"] = "o", ["ỗ"] = "o", ["ộ"] = "o", ["ơ"] = "o", ["ờ"] = "o", ["ớ"] = "o", ["ở"] = "o", ["ỡ"] = "o", ["ợ"] = "o", ["Ò"] = "O", ["Ó"] = "O", ["Ỏ"] = "O", ["Õ"] = "O", ["Ọ"] = "O", ["Ô"] = "O", ["Ồ"] = "O", ["Ố"] = "O", ["Ổ"] = "O", ["Ỗ"] = "O", ["Ộ"] = "O", ["Ơ"] = "O", ["Ờ"] = "O", ["Ớ"] = "O", ["Ở"] = "O", ["Ỡ"] = "O", ["Ợ"] = "O", ["ù"] = "u", ["ú"] = "u", ["ủ"] = "u", ["ũ"] = "u", ["ụ"] = "u", ["ư"] = "u", ["ừ"] = "u", ["ứ"] = "u", ["ử"] = "u", ["ữ"] = "u", ["ự"] = "u", ["Ù"] = "U", ["Ú"] = "U", ["Ủ"] = "U", ["Ũ"] = "U", ["Ụ"] = "U", ["Ư"] = "U", ["Ừ"] = "U", ["Ứ"] = "U", ["Ử"] = "U", ["Ữ"] = "U", ["Ự"] = "U", ["ỳ"] = "y", ["ý"] = "y", ["ỷ"] = "y", ["ỹ"] = "y", ["ỵ"] = "y", ["Ỳ"] = "Y", ["Ý"] = "Y", ["Ỷ"] = "Y", ["Ỹ"] = "Y", ["Ỵ"] = "Y" }
    local normalizeSearchText = function(text)
        local folded = text:gsub("([\194-\244][\128-\191]*)", function(ch)
            return VnFold[ch] or ch
        end)
        local expanded = folded:gsub("(%l)(%u)", "%1 %2"):lower()
        local cleaned = expanded:gsub("[^%w]+", " "):gsub("%s+", " ")
        return " " .. cleaned .. " "
    end
    local matchTextToIcon = function(text)
        if type(text) ~= "string" or text == "" then
            return nil
        end
        local padded = normalizeSearchText(text)
        for _, rule in ipairs(AutoTabRules) do
            for _, kw in ipairs(rule.keywords) do
                if padded:find(" " .. kw .. " ", 1, true) then
                    return Icons[rule.icon]
                end
            end
        end
        return nil
    end
    local resolve = function(iconInput, fallback)
        if iconInput == false then
            return ""
        end
        if type(iconInput) == "string" and iconInput:match("^%s*(.-)%s*$"):lower() == "none" then
            return ""
        end
        local resolved = getIcon(iconInput)
        if resolved then
            return resolved
        end
        return fallback or ""
    end
    local resolveTabIcon = function(rawIcon, tabTitle, tabSubtitle)
        if rawIcon == false then
            return ""
        end
        if type(rawIcon) == "string" and rawIcon:match("^%s*(.-)%s*$"):lower() == "none" then
            return ""
        end
        if rawIcon ~= nil and rawIcon ~= "" then
            local direct = getIcon(rawIcon)
            if direct then
                return direct
            end
            local fromRawText = matchTextToIcon(tostring(rawIcon))
            if fromRawText then
                return fromRawText
            end
        end
        local fromTitle = matchTextToIcon(tabTitle)
        if fromTitle then
            return fromTitle
        end
        local fromSubtitle = matchTextToIcon(tabSubtitle)
        if fromSubtitle then
            return fromSubtitle
        end
        return Icons["layout-grid"]
    end
    return {
        Icons = Icons,
        Aliases = Aliases,
        GetIcon = getIcon,
        Resolve = resolve,
        ResolveTabIcon = resolveTabIcon,
    }
end)()
VexzHub.Icons = Lucide.Icons
VexzHub.LucideIcons = Lucide.Icons
VexzHub.GetIcon = function(selfOrName, maybeName)
    if type(selfOrName) == "table" then
        return Lucide.GetIcon(maybeName)
    end
    return Lucide.GetIcon(selfOrName)
end
local TweenService = game:GetService("TweenService")
local UserInputService = game:GetService("UserInputService")
local RunService = game:GetService("RunService")
local Players = game:GetService("Players")
local SoundService = game:GetService("SoundService")
local LocalPlayer = Players.LocalPlayer
local PlayerGui = LocalPlayer:WaitForChild("PlayerGui")
local SOUND_CLICK = "rbxassetid://122954374321453"
local SOUND_TOGGLE = "rbxassetid://107978604605265"
local SOUND_OPEN = "rbxassetid://100809160609628"
local playSound = function(soundId)
    local sound = Instance.new("Sound")
    sound.SoundId = soundId
    sound.Volume = 0.6
    sound.RollOffMaxDistance = 10000
    sound.Parent = SoundService
    sound:Play()
    game:GetService("Debris"):AddItem(sound, 4)
end
local Theme = {}
Theme.Background = Color3.fromRGB(24, 24, 24)
Theme.TextWhite = Color3.fromRGB(235, 235, 235)
Theme.TextSubtitle = Color3.fromRGB(160, 160, 160)
Theme.DialogBg = Color3.fromRGB(40, 40, 40)
Theme.Border = Color3.fromRGB(55, 55, 55)
Theme.ConfigPanel = Color3.fromRGB(24, 24, 24)
Theme.TabDefault = Color3.fromRGB(24, 24, 24)
Theme.TabHover = Color3.fromRGB(40, 40, 40)
Theme.TabSelected = Color3.fromRGB(44, 44, 44)
local MutedTextColor = Color3.fromRGB(90, 90, 90)
local ColorPresets = {}
ColorPresets.Blue = {
    Accent = Color3.fromRGB(35, 85, 170),
    AccentBright = Color3.fromRGB(55, 110, 200),
    AccentDark = Color3.fromRGB(25, 65, 140),
    AccentDeep = Color3.fromRGB(18, 50, 115),
    AccentGlow = Color3.fromRGB(45, 95, 185),
}
ColorPresets.White = {
    Accent = Color3.fromRGB(200, 200, 200),
    AccentBright = Color3.fromRGB(230, 230, 230),
    AccentDark = Color3.fromRGB(155, 155, 155),
    AccentDeep = Color3.fromRGB(115, 115, 115),
    AccentGlow = Color3.fromRGB(215, 215, 215),
}
ColorPresets.Red = {
    Accent = Color3.fromRGB(170, 40, 40),
    AccentBright = Color3.fromRGB(205, 60, 60),
    AccentDark = Color3.fromRGB(130, 25, 25),
    AccentDeep = Color3.fromRGB(95, 18, 18),
    AccentGlow = Color3.fromRGB(185, 50, 50),
}
ColorPresets.Yellow = {
    Accent = Color3.fromRGB(175, 148, 30),
    AccentBright = Color3.fromRGB(212, 178, 48),
    AccentDark = Color3.fromRGB(135, 112, 20),
    AccentDeep = Color3.fromRGB(100, 83, 14),
    AccentGlow = Color3.fromRGB(192, 162, 38),
}
ColorPresets.Grey = {
    Accent = Color3.fromRGB(108, 108, 108),
    AccentBright = Color3.fromRGB(148, 148, 148),
    AccentDark = Color3.fromRGB(78, 78, 78),
    AccentDeep = Color3.fromRGB(55, 55, 55),
    AccentGlow = Color3.fromRGB(122, 122, 122),
}
ColorPresets.Green = {
    Accent = Color3.fromRGB(35, 140, 70),
    AccentBright = Color3.fromRGB(55, 175, 90),
    AccentDark = Color3.fromRGB(25, 105, 50),
    AccentDeep = Color3.fromRGB(18, 75, 35),
    AccentGlow = Color3.fromRGB(45, 155, 80),
}
ColorPresets.Purple = {
    Accent = Color3.fromRGB(110, 60, 180),
    AccentBright = Color3.fromRGB(140, 85, 215),
    AccentDark = Color3.fromRGB(85, 45, 145),
    AccentDeep = Color3.fromRGB(60, 30, 110),
    AccentGlow = Color3.fromRGB(125, 70, 195),
}
ColorPresets.Pink = {
    Accent = Color3.fromRGB(200, 70, 130),
    AccentBright = Color3.fromRGB(230, 100, 160),
    AccentDark = Color3.fromRGB(160, 50, 100),
    AccentDeep = Color3.fromRGB(120, 35, 75),
    AccentGlow = Color3.fromRGB(215, 85, 145),
}
local buildPaletteFromColor = function(accentColor)
    return {
        Accent = accentColor,
        AccentBright = accentColor:Lerp(Color3.new(1, 1, 1), 0.22),
        AccentDark = accentColor:Lerp(Color3.new(0, 0, 0), 0.1),
        AccentDeep = accentColor:Lerp(Color3.new(0, 0, 0), 0.18),
        AccentGlow = accentColor:Lerp(Color3.new(1, 1, 1), 0.08),
    }
end
local boostColorHSV = function(color, boostFactor)
    local hue, sat, val = Color3.toHSV(color)
    return Color3.fromHSV(hue, math.min(1, sat * (1 + boostFactor)), math.min(1, val * (1 + (boostFactor * 0.18))))
end
local resolveThemePalette = function(themeOrColor)
    local palette = {}
    for b5, b6 in pairs(Theme) do
        palette[b5] = b6
    end
    if typeof(themeOrColor) == "Color3" then
        for b5, b6 in pairs(buildPaletteFromColor(themeOrColor)) do
            palette[b5] = boostColorHSV(b6, 0.45)
        end
    else
        for b5, b6 in pairs(ColorPresets[themeOrColor] or ColorPresets.Red) do
            palette[b5] = boostColorHSV(b6, 0.45)
        end
    end
    return palette
end
local FontMedium = Font.new("rbxasset://fonts/families/GothamSSm.json", Enum.FontWeight.Medium)
local FontBold = Font.new("rbxasset://fonts/families/GothamSSm.json", Enum.FontWeight.Bold)
local FontRegular = Font.new("rbxasset://fonts/families/GothamSSm.json", Enum.FontWeight.Regular)
local TweenInfo035 = TweenInfo.new(0.35, Enum.EasingStyle.Quart, Enum.EasingDirection.Out)
local TweenInfo020 = TweenInfo.new(0.2, Enum.EasingStyle.Quart, Enum.EasingDirection.Out)
local TweenInfo045 = TweenInfo.new(0.45, Enum.EasingStyle.Quart, Enum.EasingDirection.Out)
local TweenInfo060 = TweenInfo.new(0.6, Enum.EasingStyle.Quart, Enum.EasingDirection.Out)
local MinWindowSize = Vector2.new(380, 250)
local MaxWindowSize = Vector2.new(900, 650)
local DefaultWindowSize = Vector2.new(520, 380)
local HEADER_HEIGHT = 48
local FOOTER_HEIGHT = 28
local CORNER_RADIUS = 6
local TAB_HEIGHT = 30
local DEFAULT_CORNER_RADIUS = 10
local ITEM_SPACING = 8
local SIDEBAR_WIDTH = 170
local ELEMENT_HEIGHT = 42
local ICON_SIZE_X = 18
local ICON_SIZE_Y = 18
local ActiveTweens = {}
local cancelGroupTweens = function(groupKey)
    if ActiveTweens[groupKey] then
        for b4, b5 in ipairs(ActiveTweens[groupKey]) do
            b5:Cancel()
        end
    end
    ActiveTweens[groupKey] = {}
end
local playGroupTween = function(groupKey, instance, tweenInfo, props)
    local tween = TweenService:Create(instance, tweenInfo, props)
    if not ActiveTweens[groupKey] then
        ActiveTweens[groupKey] = {}
    end
    table.insert(ActiveTweens[groupKey], tween)
    tween:Play()
    return tween
end
local addCorner = function(parentInstance, radius)
    local corner = Instance.new("UICorner")
    corner.CornerRadius = UDim.new(0, radius or DEFAULT_CORNER_RADIUS)
    corner.Parent = parentInstance
    return corner
end
local addStroke = function(parentInstance, color, thickness, transparency)
    local stroke = Instance.new("UIStroke")
    stroke.Color = color or Color3.fromRGB(55, 55, 55)
    stroke.Thickness = thickness or 1
    stroke.Transparency = transparency or 0.5
    stroke.Parent = parentInstance
    return stroke
end
local addPadding = function(parentInstance, top, right, bottom, left)
    local padding = Instance.new("UIPadding")
    padding.PaddingTop = UDim.new(0, top or 0)
    padding.PaddingRight = UDim.new(0, right or 0)
    padding.PaddingBottom = UDim.new(0, bottom or 0)
    padding.PaddingLeft = UDim.new(0, left or 0)
    padding.Parent = parentInstance
    return padding
end
local addShadow = function(parentInstance)
    local shadowImage = Instance.new("ImageLabel")
    shadowImage.Name = "Shadow"
    shadowImage.BackgroundTransparency = 1
    shadowImage.Image = "rbxassetid://6015897843"
    shadowImage.ImageColor3 = Color3.fromRGB(0, 0, 0)
    shadowImage.ImageTransparency = 0.5
    shadowImage.ScaleType = Enum.ScaleType.Slice
    shadowImage.SliceCenter = Rect.new(49, 49, 450, 450)
    shadowImage.Size = UDim2.new(1, 30, 1, 30)
    shadowImage.Position = UDim2.new(0, -15, 0, -15)
    shadowImage.ZIndex = -1
    shadowImage.Parent = parentInstance
    return shadowImage
end
local startMarqueeScroll = function(textLabel, clipFrame)
    local isRunning = true
    task.spawn(function()
        task.wait(0.5)
        while (((isRunning and textLabel) and textLabel.Parent) and clipFrame) and clipFrame.Parent do
            local c0 = textLabel.TextBounds.X
            local c1 = clipFrame.AbsoluteSize.X
            if c1 < c0 then
                local c2 = (c0 - c1) + 20
                local c3 = c2 / 30
                textLabel.Position = UDim2.new(0, 0, 0, 0)
                task.wait(1.5)
                if (not isRunning) or (not textLabel.Parent) then
                    break
                end
                local c4 = TweenService:Create(textLabel, TweenInfo.new(c3, Enum.EasingStyle.Linear), {
                    Position = UDim2.new(0, -c2, 0, 0),
                })
                c4:Play()
                c4.Completed:Wait()
                if (not isRunning) or (not textLabel.Parent) then
                    break
                end
                task.wait(1.2)
                textLabel.Position = UDim2.new(0, 0, 0, 0)
                task.wait(0.8)
            else
                textLabel.Position = UDim2.new(0, 0, 0, 0)
                task.wait(2)
            end
        end
    end)
    return function()
        isRunning = false
    end
end
local playLoadingScreen = function(palette, onComplete)
    local loadingGui = Instance.new("ScreenGui")
    loadingGui.Name = "VexzHubLoading"
    loadingGui.ResetOnSpawn = false
    loadingGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
    loadingGui.IgnoreGuiInset = true
    loadingGui.AutoLocalize = false
    loadingGui.DisplayOrder = 9999
    loadingGui.Parent = PlayerGui
    local backdropFrame = Instance.new("Frame")
    backdropFrame.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
    backdropFrame.BackgroundTransparency = 1
    backdropFrame.Size = UDim2.new(1, 0, 1, 0)
    backdropFrame.ZIndex = 1
    backdropFrame.Parent = loadingGui
    local cardSize = 160
    local cardFrame = Instance.new("Frame")
    cardFrame.BackgroundColor3 = Theme.Background
    cardFrame.BackgroundTransparency = 1
    cardFrame.AnchorPoint = Vector2.new(0.5, 0.5)
    cardFrame.Size = UDim2.new(0, cardSize, 0, cardSize)
    cardFrame.Position = UDim2.new(0.5, 0, 0.5, 0)
    cardFrame.ClipsDescendants = false
    cardFrame.ZIndex = 2
    cardFrame.Parent = loadingGui
    local addCardCorner = function(c0, c1)
        local c2 = Instance.new("UICorner")
        c2.CornerRadius = UDim.new(0, c1 or 10)
        c2.Parent = c0
        return c2
    end
    local addCardStroke = function(c0, c1, c2, c3)
        local c4 = Instance.new("UIStroke")
        c4.Color = c1 or Color3.fromRGB(55, 55, 55)
        c4.Thickness = c2 or 1
        c4.Transparency = c3 or 0.5
        c4.Parent = c0
        return c4
    end
    local addCardShadow = function(c0)
        local c1 = Instance.new("ImageLabel")
        c1.Name = "Shadow"
        c1.BackgroundTransparency = 1
        c1.Image = "rbxassetid://6015897843"
        c1.ImageColor3 = Color3.fromRGB(0, 0, 0)
        c1.ImageTransparency = 0.5
        c1.ScaleType = Enum.ScaleType.Slice
        c1.SliceCenter = Rect.new(49, 49, 450, 450)
        c1.Size = UDim2.new(1, 30, 1, 30)
        c1.Position = UDim2.new(0, -15, 0, -15)
        c1.ZIndex = -1
        c1.Parent = c0
        return c1
    end
    addCardCorner(cardFrame, 18)
    local cardStroke = addCardStroke(cardFrame, Theme.Border, 1, 1)
    local cardShadow = addCardShadow(cardFrame)
    cardShadow.ImageTransparency = 1
    local cardScale = Instance.new("UIScale")
    cardScale.Scale = 0.72
    cardScale.Parent = cardFrame
    local ringContainerSize = 96
    local ringRadius = 34
    local ringStepDeg = 90
    local numDots = 52
    local baseDotSize = 5
    local ringFrame = Instance.new("Frame")
    ringFrame.BackgroundTransparency = 1
    ringFrame.AnchorPoint = Vector2.new(0.5, 0.5)
    ringFrame.Size = UDim2.new(0, ringContainerSize, 0, ringContainerSize)
    ringFrame.Position = UDim2.new(0.5, 0, 0.5, 0)
    ringFrame.ZIndex = 3
    ringFrame.Parent = cardFrame
    local ringTrack = Instance.new("Frame")
    ringTrack.BackgroundTransparency = 1
    ringTrack.AnchorPoint = Vector2.new(0.5, 0.5)
    ringTrack.Size = UDim2.new(0, (ringRadius * 2) + 2, 0, (ringRadius * 2) + 2)
    ringTrack.Position = UDim2.new(0.5, 0, 0.5, 0)
    ringTrack.ZIndex = 2
    ringTrack.Parent = ringFrame
    local ringStroke = Instance.new("UIStroke")
    ringStroke.Color = Theme.Border
    ringStroke.Thickness = 1.5
    ringStroke.Transparency = 0.6
    ringStroke.Parent = ringTrack
    Instance.new("UICorner", ringTrack).CornerRadius = UDim.new(1, 0)
    local centerX = ringContainerSize / 2
    local centerY = ringContainerSize / 2
    local dotFrames = {}
    local headGlowInner = nil
    local headGlowOuter = nil
    for b28 = 0, numDots - 1 do
        local b29 = math.rad(b28 * (360 / ringStepDeg))
        local b30 = centerX + (ringRadius * math.sin(b29))
        local b31 = centerY - (ringRadius * math.cos(b29))
        local b32 = b28 / (numDots - 1)
        local b33 = nil
        local b34 = nil
        local b35 = nil
        if b28 == 0 then
            b35 = baseDotSize + 3
            b33 = Color3.new(1, 1, 1)
            b34 = 0
        elseif b32 < 0.12 then
            local b36 = b32 / 0.12
            b35 = baseDotSize + math.round((1 - b36) * 2)
            b33 = Color3.new(1, 1, 1):Lerp(palette.AccentBright, b36)
            b34 = b36 * 0.04
        elseif b32 < 0.4 then
            local b36 = (b32 - 0.12) / 0.28
            b35 = baseDotSize
            b33 = palette.AccentBright:Lerp(palette.Accent, b36)
            b34 = 0.04 + (b36 * 0.32)
        elseif b32 < 0.68 then
            local b36 = (b32 - 0.4) / 0.28
            b35 = baseDotSize
            b33 = palette.Accent:Lerp(palette.AccentDark, b36)
            b34 = 0.36 + (b36 * 0.38)
        else
            local b36 = (b32 - 0.68) / 0.32
            b35 = math.max(3, baseDotSize - math.floor(b36 * 2))
            b33 = palette.AccentDark
            b34 = 0.74 + (b36 * 0.26)
        end
        local b36 = Instance.new("Frame")
        b36.BackgroundColor3 = b33
        b36.BackgroundTransparency = b34
        b36.BorderSizePixel = 0
        b36.Size = UDim2.new(0, b35, 0, b35)
        b36.Position = UDim2.new(0, b30 - (b35 / 2), 0, b31 - (b35 / 2))
        b36.ZIndex = 4
        b36.Parent = ringFrame
        Instance.new("UICorner", b36).CornerRadius = UDim.new(1, 0)
        table.insert(dotFrames, b36)
        if b28 == 0 then
            local b37 = baseDotSize + 12
            headGlowInner = Instance.new("Frame")
            headGlowInner.BackgroundColor3 = palette.AccentBright
            headGlowInner.BackgroundTransparency = 0.5
            headGlowInner.BorderSizePixel = 0
            headGlowInner.Size = UDim2.new(0, b37, 0, b37)
            headGlowInner.Position = UDim2.new(0.5, -b37 / 2, 0.5, -b37 / 2)
            headGlowInner.ZIndex = 3
            headGlowInner.Parent = b36
            Instance.new("UICorner", headGlowInner).CornerRadius = UDim.new(1, 0)
            local b38 = baseDotSize + 24
            headGlowOuter = Instance.new("Frame")
            headGlowOuter.BackgroundColor3 = palette.Accent
            headGlowOuter.BackgroundTransparency = 0.82
            headGlowOuter.BorderSizePixel = 0
            headGlowOuter.Size = UDim2.new(0, b38, 0, b38)
            headGlowOuter.Position = UDim2.new(0.5, -b38 / 2, 0.5, -b38 / 2)
            headGlowOuter.ZIndex = 2
            headGlowOuter.Parent = b36
            Instance.new("UICorner", headGlowOuter).CornerRadius = UDim.new(1, 0)
            task.spawn(function()
                local c0 = TweenInfo.new(0.6, Enum.EasingStyle.Sine, Enum.EasingDirection.InOut)
                while headGlowInner and headGlowInner.Parent do
                    TweenService:Create(headGlowInner, c0, {
                        BackgroundTransparency = 0.28,
                    }):Play()
                    task.wait(0.6)
                    TweenService:Create(headGlowInner, c0, {
                        BackgroundTransparency = 0.58,
                    }):Play()
                    task.wait(0.6)
                end
            end)
        end
    end
    task.delay(0.05, function()
        TweenService:Create(backdropFrame, TweenInfo045, {
            BackgroundTransparency = 0.6,
        }):Play()
        TweenService:Create(cardFrame, TweenInfo045, {
            BackgroundTransparency = 0,
        }):Play()
        TweenService:Create(cardStroke, TweenInfo045, {
            Transparency = 0.45,
        }):Play()
        TweenService:Create(cardShadow, TweenInfo060, {
            ImageTransparency = 0.45,
        }):Play()
        TweenService:Create(cardScale, TweenInfo.new(0.5, Enum.EasingStyle.Back, Enum.EasingDirection.Out), {
            Scale = 1,
        }):Play()
    end)
    local isSpinning = true
    local heartbeatConn = RunService.Heartbeat:Connect(function(c0)
        if not isSpinning then
            return
        end
        ringFrame.Rotation = ringFrame.Rotation - (c0 * 220)
    end)
    task.delay(2.8, function()
        isSpinning = false
        heartbeatConn:Disconnect()
        local c0 = TweenInfo.new(0.2, Enum.EasingStyle.Quart, Enum.EasingDirection.Out)
        for c4, c5 in ipairs(dotFrames) do
            TweenService:Create(c5, c0, {
                BackgroundTransparency = 1,
            }):Play()
            for c9, c10 in ipairs(c5:GetChildren()) do
                if c10:IsA("Frame") then
                    TweenService:Create(c10, c0, {
                        BackgroundTransparency = 1,
                    }):Play()
                end
            end
        end
        TweenService:Create(ringStroke, c0, {
            Transparency = 1,
        }):Play()
        local c1 = TweenInfo.new(0.32, Enum.EasingStyle.Quart, Enum.EasingDirection.In)
        task.delay(0.14, function()
            TweenService:Create(cardScale, c1, {
                Scale = 0.82,
            }):Play()
            TweenService:Create(cardFrame, c1, {
                BackgroundTransparency = 1,
            }):Play()
            TweenService:Create(cardStroke, c1, {
                Transparency = 1,
            }):Play()
            TweenService:Create(cardShadow, c1, {
                ImageTransparency = 1,
            }):Play()
        end)
        task.delay(0.22, function()
            TweenService:Create(backdropFrame, c1, {
                BackgroundTransparency = 1,
            }):Play()
        end)
        task.delay(0.62, function()
            loadingGui:Destroy()
            if onComplete then
                onComplete()
            end
        end)
    end)
end
VexzHub.new = function()
    local instance = setmetatable({}, VexzHub)
    instance._connections = {}
    instance._windows = {}
    return instance
end
VexzHub.Notify = function(self, c0)
    c0 = c0 or {}
    if self and self._showNotification then
        self._showNotification(c0)
    end
end
VexzHub.NewWindow = function(self, windowOpts)
    windowOpts = windowOpts or {}
    local windowTitle = windowOpts.Title or "VexzHub"
    local windowSubtitle = windowOpts.Subtitle or "Blox Fruits"
    local windowIcon = ((windowOpts.Icon == "") and "") or Lucide.Resolve(windowOpts.Icon, "rbxassetid://81844334586058")
    local windowSize = windowOpts.Size or DefaultWindowSize
    local palette = resolveThemePalette(windowOpts.Theme or "Red")
    local winState = {}
    winState.minimized = false
    winState.maximized = false
    winState.configOpen = false
    winState.hidden = false
    winState.acrylicEnabled = false
    winState.acrylicOpacity = 0.55
    winState.wallpaperOpacity = 0.75
    winState.backgroundImageId = ""
    winState.customColorHex = ""
    winState.preMaxSize = nil
    winState.preMaxPos = nil
    winState.preMinSize = nil
    winState.dragging = false
    winState.resizing = false
    winState.destroyed = false
    winState.connections = {}
    winState.tabs = {}
    winState.selectedTab = nil
    winState.accentElems = {}
    winState.themeCallbacks = {}
    winState.titleSegments = {}
    winState.searchRegistry = {}
    winState.componentRegistry = {}
    winState.loadedComponentState = {}
    local deferredLoaders = {}
    local bindThemeProp = function(c0, c1, c2)
        table.insert(winState.accentElems, {
            inst = c0,
            prop = c1,
            key = c2,
        })
    end
    local onThemeChange = function(c0)
        table.insert(winState.themeCallbacks, c0)
    end
    local registerComponent = function(c0, c1, c2)
        if (not c0) or (c0 == "") then
            return
        end
        winState.componentRegistry[c0] = {
            kind = c1,
            object = c2,
        }
        local c3 = winState.loadedComponentState[c0]
        if c3 ~= nil then
            table.insert(deferredLoaders, function()
                pcall(function()
                    c2:Set(c3)
                end)
            end)
        end
    end
    local applyHoverGlow = function(c0, c1)
        addCorner(c0, 6)
        local c2 = Instance.new("UIStroke")
        c2.Color = palette.Accent
        c2.Thickness = 1
        c2.Transparency = 1
        c2.Parent = c0
        c0.InputBegan:Connect(function(d0)
            if d0.UserInputType == Enum.UserInputType.MouseMovement then
                c2.Color = palette.Accent
                cancelGroupTweens(c1 .. "_glow")
                playGroupTween(c1 .. "_glow", c2, TweenInfo020, {
                    Transparency = 0.55,
                })
            end
        end)
        c0.InputEnded:Connect(function(d0)
            if d0.UserInputType == Enum.UserInputType.MouseMovement then
                cancelGroupTweens(c1 .. "_glow")
                playGroupTween(c1 .. "_glow", c2, TweenInfo020, {
                    Transparency = 1,
                })
            end
        end)
        return c2
    end
    for b16, b17 in ipairs(PlayerGui:GetChildren()) do
        if ((b17.Name == "VexzHubUI") or (b17.Name == "VexzHubFloat")) or (b17.Name == "VexzHubNotify") then
            b17:Destroy()
        end
    end
    local screenGui = Instance.new("ScreenGui")
    screenGui.Name = "VexzHubUI"
    screenGui.ResetOnSpawn = false
    screenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
    screenGui.IgnoreGuiInset = true
    screenGui.AutoLocalize = false
    screenGui.Parent = PlayerGui
    local mainFrame = Instance.new("Frame")
    mainFrame.Name = "Window"
    mainFrame.BackgroundColor3 = palette.Background
    mainFrame.Size = UDim2.new(0, windowSize.X, 0, 0)
    mainFrame.Position = UDim2.new(0.5, -windowSize.X / 2, 0.5, ICON_SIZE_Y - (windowSize.Y / 2))
    mainFrame.BackgroundTransparency = 1
    mainFrame.ClipsDescendants = true
    mainFrame.Visible = false
    mainFrame.Parent = screenGui
    addCorner(mainFrame, DEFAULT_CORNER_RADIUS)
    local mainStroke = addStroke(mainFrame, Color3.fromRGB(55, 55, 55), 1, 1)
    local mainShadow = addShadow(mainFrame)
    mainShadow.ImageTransparency = 1
    local wallpaperImage = Instance.new("ImageLabel")
    wallpaperImage.Name = "ThemeBackground"
    wallpaperImage.BackgroundTransparency = 1
    wallpaperImage.Size = UDim2.new(1, 0, 1, 0)
    wallpaperImage.Position = UDim2.new(0, 0, 0, 0)
    wallpaperImage.ZIndex = 0
    wallpaperImage.ScaleType = Enum.ScaleType.Crop
    wallpaperImage.ClipsDescendants = true
    wallpaperImage.ImageTransparency = 1 - winState.wallpaperOpacity
    wallpaperImage.Visible = false
    wallpaperImage.Image = ""
    wallpaperImage.Parent = mainFrame
    addCorner(wallpaperImage, DEFAULT_CORNER_RADIUS)
    local modalOverlay = Instance.new("Frame")
    modalOverlay.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
    modalOverlay.BackgroundTransparency = 1
    modalOverlay.Size = UDim2.new(1, 0, 1, 0)
    modalOverlay.ZIndex = 50
    modalOverlay.Visible = false
    modalOverlay.Parent = mainFrame
    addCorner(modalOverlay, DEFAULT_CORNER_RADIUS)
    local contentHolder = Instance.new("Frame")
    contentHolder.BackgroundTransparency = 1
    contentHolder.Size = UDim2.new(1, 0, 0, HEADER_HEIGHT)
    contentHolder.BorderSizePixel = 0
    contentHolder.ZIndex = 5
    contentHolder.Parent = mainFrame
    local headerFrame = Instance.new("Frame")
    headerFrame.BackgroundColor3 = palette.Border
    headerFrame.BackgroundTransparency = 0.7
    headerFrame.Size = UDim2.new(0.92, 0, 0, 1)
    headerFrame.Position = UDim2.new(0.04, 0, 1, 0)
    headerFrame.BorderSizePixel = 0
    headerFrame.ZIndex = 6
    headerFrame.Parent = contentHolder
    bindThemeProp(headerFrame, "BackgroundColor3", "Border")
    local headerLeftFrame = Instance.new("Frame")
    headerLeftFrame.BackgroundTransparency = 1
    headerLeftFrame.Size = UDim2.new(0.6, 0, 1, 0)
    headerLeftFrame.ZIndex = 6
    headerLeftFrame.Parent = contentHolder
    local headerLeftLayout = Instance.new("UIListLayout")
    headerLeftLayout.FillDirection = Enum.FillDirection.Horizontal
    headerLeftLayout.VerticalAlignment = Enum.VerticalAlignment.Center
    headerLeftLayout.Padding = UDim.new(0, 8)
    headerLeftLayout.SortOrder = Enum.SortOrder.LayoutOrder
    headerLeftLayout.Parent = headerLeftFrame
    addPadding(headerLeftFrame, 0, 0, 0, 12)
    if windowIcon ~= "" then
        local b23 = Instance.new("ImageLabel")
        b23.BackgroundTransparency = 1
        b23.Size = UDim2.new(0, TAB_HEIGHT, 0, TAB_HEIGHT)
        b23.Image = windowIcon
        b23.ImageColor3 = Color3.new(1, 1, 1)
        b23.LayoutOrder = 1
        b23.ZIndex = 7
        b23.Parent = headerLeftFrame
        addCorner(b23, 6)
    end
    local titleStackFrame = Instance.new("Frame")
    titleStackFrame.BackgroundTransparency = 1
    titleStackFrame.Size = UDim2.new(0, 200, 1, 0)
    titleStackFrame.AutomaticSize = Enum.AutomaticSize.X
    titleStackFrame.LayoutOrder = 2
    titleStackFrame.ZIndex = 7
    titleStackFrame.Parent = headerLeftFrame
    local titleStackLayout = Instance.new("UIListLayout")
    titleStackLayout.FillDirection = Enum.FillDirection.Vertical
    titleStackLayout.VerticalAlignment = Enum.VerticalAlignment.Center
    titleStackLayout.Padding = UDim.new(0, 1)
    titleStackLayout.SortOrder = Enum.SortOrder.LayoutOrder
    titleStackLayout.Parent = titleStackFrame
    local titleRowFrame = Instance.new("Frame")
    titleRowFrame.BackgroundTransparency = 1
    titleRowFrame.Size = UDim2.new(1, 0, 0, 18)
    titleRowFrame.AutomaticSize = Enum.AutomaticSize.X
    titleRowFrame.LayoutOrder = 1
    titleRowFrame.ZIndex = 7
    titleRowFrame.Parent = titleStackFrame
    local titleRowLayout = Instance.new("UIListLayout")
    titleRowLayout.FillDirection = Enum.FillDirection.Horizontal
    titleRowLayout.VerticalAlignment = Enum.VerticalAlignment.Center
    titleRowLayout.Padding = UDim.new(0, 4)
    titleRowLayout.SortOrder = Enum.SortOrder.LayoutOrder
    titleRowLayout.Parent = titleRowFrame
    local titleTextLabel = Instance.new("TextLabel")
    titleTextLabel.BackgroundTransparency = 1
    titleTextLabel.Size = UDim2.new(0, 0, 1, 0)
    titleTextLabel.AutomaticSize = Enum.AutomaticSize.X
    titleTextLabel.FontFace = FontBold
    titleTextLabel.TextSize = 15
    titleTextLabel.TextXAlignment = Enum.TextXAlignment.Left
    titleTextLabel.LayoutOrder = 1
    titleTextLabel.ZIndex = 8
    titleTextLabel.Text = windowTitle
    titleTextLabel.TextColor3 = Color3.new(1, 1, 1)
    titleTextLabel.Parent = titleRowFrame
    local titleGradient = Instance.new("UIGradient")
    titleGradient.Color = ColorSequence.new({
        ColorSequenceKeypoint.new(0, Color3.new(1, 1, 1)),
        ColorSequenceKeypoint.new(1, palette.AccentBright),
    })
    titleGradient.Rotation = 100
    titleGradient.Parent = titleTextLabel
    onThemeChange(function()
        titleGradient.Color = ColorSequence.new({
            ColorSequenceKeypoint.new(0, Color3.new(1, 1, 1)),
            ColorSequenceKeypoint.new(1, palette.AccentBright),
        })
    end)
    local subtitleTextLabel = Instance.new("TextLabel")
    subtitleTextLabel.BackgroundTransparency = 1
    subtitleTextLabel.Size = UDim2.new(1, 0, 0, 13)
    subtitleTextLabel.AutomaticSize = Enum.AutomaticSize.X
    subtitleTextLabel.FontFace = FontMedium
    subtitleTextLabel.TextSize = 11
    subtitleTextLabel.TextColor3 = palette.TextSubtitle
    subtitleTextLabel.TextTransparency = 0.3
    subtitleTextLabel.TextXAlignment = Enum.TextXAlignment.Left
    subtitleTextLabel.Text = windowSubtitle
    subtitleTextLabel.LayoutOrder = 2
    subtitleTextLabel.ZIndex = 8
    subtitleTextLabel.Parent = titleStackFrame
    bindThemeProp(subtitleTextLabel, "TextColor3", "TextSubtitle")
    local headerRightFrame = Instance.new("Frame")
    headerRightFrame.BackgroundTransparency = 1
    headerRightFrame.Size = UDim2.new(0.4, 0, 1, 0)
    headerRightFrame.Position = UDim2.new(0.6, 0, 0, 0)
    headerRightFrame.ZIndex = 6
    headerRightFrame.Parent = contentHolder
    local headerRightLayout = Instance.new("UIListLayout")
    headerRightLayout.FillDirection = Enum.FillDirection.Horizontal
    headerRightLayout.HorizontalAlignment = Enum.HorizontalAlignment.Right
    headerRightLayout.VerticalAlignment = Enum.VerticalAlignment.Center
    headerRightLayout.Padding = UDim.new(0, CORNER_RADIUS)
    headerRightLayout.SortOrder = Enum.SortOrder.LayoutOrder
    headerRightLayout.Parent = headerRightFrame
    addPadding(headerRightFrame, 0, 12, 0, 0)
    local headerButtonDefs = {
        {
            name = "Config",
            icon = "rbxassetid://123669217353469",
            order = 1,
        },
        {
            name = "Minimize",
            icon = "rbxassetid://72319180199150",
            order = 2,
        },
        {
            name = "Maximize",
            icon = "rbxassetid://100039729329934",
            order = 3,
        },
        {
            name = "Close",
            icon = "rbxassetid://113006594954898",
            order = 4,
        },
    }
    local headerButtons = {}
    local headerBtnIcons = {}
    for b38, b39 in ipairs(headerButtonDefs) do
        local b40 = Instance.new("ImageButton")
        b40.BackgroundColor3 = palette.Background
        b40.BackgroundTransparency = 0.5
        b40.Size = UDim2.new(0, FOOTER_HEIGHT, 0, FOOTER_HEIGHT)
        b40.LayoutOrder = b39.order
        b40.AutoButtonColor = false
        b40.ZIndex = 7
        b40.Parent = headerRightFrame
        addCorner(b40, 6)
        local b41 = addStroke(b40, palette.Border, 1, 0.6)
        bindThemeProp(b40, "BackgroundColor3", "Background")
        onThemeChange(function()
            b41.Color = palette.Border
        end)
        local b42 = Instance.new("ImageLabel")
        b42.BackgroundTransparency = 1
        b42.Size = UDim2.new(0, 16, 0, 16)
        b42.Position = UDim2.new(0.5, -8, 0.5, -8)
        b42.Image = b39.icon
        b42.ImageColor3 = palette.Accent
        b42.ZIndex = 8
        b42.Parent = b40
        headerBtnIcons[b39.name] = b42
        local b43 = "btn_" .. b39.name
        table.insert(winState.connections, b40.MouseEnter:Connect(function()
            cancelGroupTweens(b43)
            playGroupTween(b43, b42, TweenInfo020, {
                Size = UDim2.new(0, 20, 0, 20),
                Position = UDim2.new(0.5, -10, 0.5, -10),
                ImageColor3 = palette.AccentBright,
            })
            playGroupTween(b43, b40, TweenInfo020, {
                BackgroundTransparency = 0.15,
            })
            playGroupTween(b43, b41, TweenInfo020, {
                Transparency = 0.2,
                Color = palette.Accent,
            })
        end))
        table.insert(winState.connections, b40.MouseLeave:Connect(function()
            cancelGroupTweens(b43)
            playGroupTween(b43, b42, TweenInfo020, {
                Size = UDim2.new(0, 16, 0, 16),
                Position = UDim2.new(0.5, -8, 0.5, -8),
                ImageColor3 = palette.Accent,
            })
            playGroupTween(b43, b40, TweenInfo020, {
                BackgroundTransparency = 0.5,
            })
            playGroupTween(b43, b41, TweenInfo020, {
                Transparency = 0.6,
                Color = palette.Border,
            })
        end))
        headerButtons[b39.name] = b40
    end
    local footerFrame = Instance.new("Frame")
    footerFrame.BackgroundTransparency = 1
    footerFrame.Size = UDim2.new(0, 0, 1, 0)
    footerFrame.AutomaticSize = Enum.AutomaticSize.X
    footerFrame.AnchorPoint = Vector2.new(0.5, 0)
    footerFrame.Position = UDim2.new(0.5, 0, 0, 0)
    footerFrame.ZIndex = 6
    footerFrame.Visible = false
    footerFrame.Parent = contentHolder
    local footerLayout = Instance.new("UIListLayout")
    footerLayout.FillDirection = Enum.FillDirection.Vertical
    footerLayout.VerticalAlignment = Enum.VerticalAlignment.Center
    footerLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center
    footerLayout.Padding = UDim.new(0, 1)
    footerLayout.SortOrder = Enum.SortOrder.LayoutOrder
    footerLayout.Parent = footerFrame
    local fpsLabel = Instance.new("TextLabel")
    fpsLabel.BackgroundTransparency = 1
    fpsLabel.Size = UDim2.new(1, 0, 0, 0)
    fpsLabel.AutomaticSize = Enum.AutomaticSize.Y
    fpsLabel.FontFace = FontBold
    fpsLabel.TextSize = 13
    fpsLabel.TextColor3 = palette.AccentBright
    fpsLabel.Text = "FPS: -"
    fpsLabel.TextXAlignment = Enum.TextXAlignment.Center
    fpsLabel.LayoutOrder = 1
    fpsLabel.ZIndex = 7
    fpsLabel.Visible = false
    fpsLabel.Parent = footerFrame
    bindThemeProp(fpsLabel, "TextColor3", "AccentBright")
    local pingLabel = Instance.new("TextLabel")
    pingLabel.BackgroundTransparency = 1
    pingLabel.Size = UDim2.new(1, 0, 0, 0)
    pingLabel.AutomaticSize = Enum.AutomaticSize.Y
    pingLabel.FontFace = FontBold
    pingLabel.TextSize = 13
    pingLabel.TextColor3 = palette.AccentBright
    pingLabel.Text = "PING: -"
    pingLabel.TextXAlignment = Enum.TextXAlignment.Center
    pingLabel.LayoutOrder = 2
    pingLabel.ZIndex = 7
    pingLabel.Visible = false
    pingLabel.Parent = footerFrame
    bindThemeProp(pingLabel, "TextColor3", "AccentBright")
    local showFps = false
    local showPing = false
    local showProfile = false
    local fpsFrameCount = 0
    local fpsElapsed = 0
    local updateFooterVisibility = function()
        footerFrame.Visible = showFps or showPing
        fpsLabel.Visible = showFps
        pingLabel.Visible = showPing
    end
    table.insert(winState.connections, RunService.Heartbeat:Connect(function(c0)
        fpsFrameCount = fpsFrameCount + 1
        fpsElapsed = fpsElapsed + c0
        if fpsElapsed >= 0.5 then
            if showFps then
                fpsLabel.Text = "FPS: " .. tostring(math.floor(fpsFrameCount / fpsElapsed))
            end
            if showPing then
                pingLabel.Text = "PING: " .. tostring(math.floor(Players.LocalPlayer:GetNetworkPing() * 1000)) .. "ms"
            end
            fpsFrameCount = 0
            fpsElapsed = 0
        end
    end))
    local searchBarHeight = 34
    local searchBoxContainer = Instance.new("Frame")
    searchBoxContainer.BackgroundColor3 = palette.Background
    searchBoxContainer.BackgroundTransparency = 0.75
    searchBoxContainer.Size = UDim2.new(0, SIDEBAR_WIDTH, 0, searchBarHeight)
    searchBoxContainer.Position = UDim2.new(0, 0, 0, HEADER_HEIGHT + 1)
    searchBoxContainer.BorderSizePixel = 0
    searchBoxContainer.ZIndex = 4
    searchBoxContainer.ClipsDescendants = true
    searchBoxContainer.Parent = mainFrame
    bindThemeProp(searchBoxContainer, "BackgroundColor3", "Background")
    local searchIcon = Instance.new("ImageLabel")
    searchIcon.BackgroundTransparency = 1
    searchIcon.Size = UDim2.new(0, 14, 0, 14)
    searchIcon.Position = UDim2.new(0, 9, 0.5, -7)
    searchIcon.Image = "rbxassetid://115739298989740"
    searchIcon.ImageColor3 = palette.TextSubtitle
    searchIcon.ZIndex = 5
    searchIcon.Parent = searchBoxContainer
    local searchTextBox = Instance.new("TextBox")
    searchTextBox.BackgroundTransparency = 1
    searchTextBox.Size = UDim2.new(1, -32, 1, 0)
    searchTextBox.Position = UDim2.new(0, 28, 0, 0)
    searchTextBox.FontFace = FontMedium
    searchTextBox.TextSize = 11
    searchTextBox.TextColor3 = palette.TextWhite
    searchTextBox.PlaceholderColor3 = palette.TextSubtitle
    searchTextBox.PlaceholderText = "Search..."
    searchTextBox.TextXAlignment = Enum.TextXAlignment.Left
    searchTextBox.ClearTextOnFocus = false
    searchTextBox.Text = ""
    searchTextBox.ZIndex = 5
    searchTextBox.Parent = searchBoxContainer
    bindThemeProp(searchTextBox, "TextColor3", "TextWhite")
    bindThemeProp(searchTextBox, "PlaceholderColor3", "TextSubtitle")
    local bodyContainer = Instance.new("Frame")
    bodyContainer.BackgroundColor3 = palette.Border
    bodyContainer.BackgroundTransparency = 0.5
    bodyContainer.Size = UDim2.new(1, 0, 0, 1)
    bodyContainer.Position = UDim2.new(0, 0, 1, -1)
    bodyContainer.BorderSizePixel = 0
    bodyContainer.ZIndex = 5
    bodyContainer.Parent = searchBoxContainer
    bindThemeProp(bodyContainer, "BackgroundColor3", "Border")
    local tabListScroll = Instance.new("ScrollingFrame")
    tabListScroll.BackgroundTransparency = 1
    tabListScroll.Size = UDim2.new(0, SIDEBAR_WIDTH, 1, (-HEADER_HEIGHT - 1) - searchBarHeight)
    tabListScroll.Position = UDim2.new(0, 0, 0, (HEADER_HEIGHT + 1) + searchBarHeight)
    tabListScroll.BorderSizePixel = 0
    tabListScroll.ScrollBarThickness = 2
    tabListScroll.ScrollBarImageColor3 = MutedTextColor
    tabListScroll.ScrollBarImageTransparency = 0.5
    tabListScroll.CanvasSize = UDim2.new(0, 0, 0, 0)
    tabListScroll.AutomaticCanvasSize = Enum.AutomaticSize.Y
    tabListScroll.ClipsDescendants = true
    tabListScroll.ZIndex = 3
    tabListScroll.Parent = mainFrame
    local tabListLayout = Instance.new("UIListLayout")
    tabListLayout.FillDirection = Enum.FillDirection.Vertical
    tabListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center
    tabListLayout.Padding = UDim.new(0, 2)
    tabListLayout.SortOrder = Enum.SortOrder.LayoutOrder
    tabListLayout.Parent = tabListScroll
    addPadding(tabListScroll, 4, 4, 4, 4)
    local sidebarDivider = Instance.new("Frame")
    sidebarDivider.BackgroundColor3 = palette.Border
    sidebarDivider.BackgroundTransparency = 0.7
    sidebarDivider.Size = UDim2.new(0, 1, 1, -HEADER_HEIGHT - 12)
    sidebarDivider.Position = UDim2.new(0, SIDEBAR_WIDTH, 0, HEADER_HEIGHT + 6)
    sidebarDivider.BorderSizePixel = 0
    sidebarDivider.ZIndex = 3
    sidebarDivider.Parent = mainFrame
    bindThemeProp(sidebarDivider, "BackgroundColor3", "Border")
    local pagesContainer = Instance.new("Frame")
    pagesContainer.BackgroundTransparency = 1
    pagesContainer.Size = UDim2.new(1, -SIDEBAR_WIDTH - 1, 1, -HEADER_HEIGHT)
    pagesContainer.Position = UDim2.new(0, SIDEBAR_WIDTH + 1, 0, HEADER_HEIGHT)
    pagesContainer.ClipsDescendants = true
    pagesContainer.ZIndex = 2
    pagesContainer.Parent = mainFrame
    local searchResultsScroll = Instance.new("ScrollingFrame")
    searchResultsScroll.BackgroundTransparency = 1
    searchResultsScroll.Size = UDim2.new(1, -SIDEBAR_WIDTH - 1, 1, -HEADER_HEIGHT)
    searchResultsScroll.Position = UDim2.new(0, SIDEBAR_WIDTH + 1, 0, HEADER_HEIGHT)
    searchResultsScroll.Visible = false
    searchResultsScroll.ZIndex = 10
    searchResultsScroll.BorderSizePixel = 0
    searchResultsScroll.ScrollBarThickness = 2
    searchResultsScroll.ScrollBarImageColor3 = MutedTextColor
    searchResultsScroll.ScrollBarImageTransparency = 0.5
    searchResultsScroll.CanvasSize = UDim2.new(0, 0, 0, 0)
    searchResultsScroll.AutomaticCanvasSize = Enum.AutomaticSize.Y
    searchResultsScroll.ClipsDescendants = false
    searchResultsScroll.Parent = mainFrame
    local searchResultsLayout = Instance.new("UIListLayout")
    searchResultsLayout.FillDirection = Enum.FillDirection.Vertical
    searchResultsLayout.Padding = UDim.new(0, 6)
    searchResultsLayout.SortOrder = Enum.SortOrder.LayoutOrder
    searchResultsLayout.Parent = searchResultsScroll
    addPadding(searchResultsScroll, 10, 12, 10, 12)
    local resizeHandle = Instance.new("TextButton")
    resizeHandle.BackgroundTransparency = 1
    resizeHandle.Size = UDim2.new(0, 18, 0, 18)
    resizeHandle.Position = UDim2.new(1, -18, 1, -18)
    resizeHandle.Text = ""
    resizeHandle.ZIndex = 100
    resizeHandle.AutoButtonColor = false
    resizeHandle.Parent = mainFrame
    local resizeGripDot = Instance.new("Frame")
    resizeGripDot.BackgroundTransparency = 1
    resizeGripDot.Size = UDim2.new(1, -4, 1, -4)
    resizeGripDot.Position = UDim2.new(0, 4, 0, 4)
    resizeGripDot.ZIndex = 101
    resizeGripDot.Parent = resizeHandle
    local configCardStrokes = {}
    for b63 = 0, 2 do
        for b67 = 0, 2 do
            if (b63 + b67) >= 2 then
                local b68 = Instance.new("Frame")
                b68.BackgroundColor3 = palette.Accent
                b68.BackgroundTransparency = 0.5
                b68.Size = UDim2.new(0, 2, 0, 2)
                b68.Position = UDim2.new(0, b67 * 5, 0, b63 * 5)
                b68.BorderSizePixel = 0
                b68.ZIndex = 102
                b68.Parent = resizeGripDot
                addCorner(b68, 1)
                table.insert(configCardStrokes, b68)
                bindThemeProp(b68, "BackgroundColor3", "Accent")
            end
        end
    end
    local configDrawer = Instance.new("ScrollingFrame")
    configDrawer.BackgroundColor3 = palette.ConfigPanel
    configDrawer.Size = UDim2.new(0, 220, 0, 400)
    configDrawer.ZIndex = 200
    configDrawer.ClipsDescendants = true
    configDrawer.Visible = false
    configDrawer.BorderSizePixel = 0
    configDrawer.ScrollBarThickness = 2
    configDrawer.ScrollBarImageColor3 = MutedTextColor
    configDrawer.ScrollBarImageTransparency = 0.6
    configDrawer.CanvasSize = UDim2.new(0, 0, 0, 0)
    configDrawer.AutomaticCanvasSize = Enum.AutomaticSize.Y
    configDrawer.Parent = screenGui
    addCorner(configDrawer, ITEM_SPACING)
    local configDrawerStroke = addStroke(configDrawer, palette.Border, 1, 0.5)
    bindThemeProp(configDrawer, "BackgroundColor3", "ConfigPanel")
    bindThemeProp(configDrawerStroke, "Color", "Border")
    local configDrawerLayout = Instance.new("UIListLayout")
    configDrawerLayout.FillDirection = Enum.FillDirection.Vertical
    configDrawerLayout.Padding = UDim.new(0, 6)
    configDrawerLayout.SortOrder = Enum.SortOrder.LayoutOrder
    configDrawerLayout.Parent = configDrawer
    addPadding(configDrawer, 12, 12, 40, 12)
    local configHeaderLabel = Instance.new("TextLabel")
    configHeaderLabel.BackgroundTransparency = 1
    configHeaderLabel.Size = UDim2.new(1, 0, 0, 24)
    configHeaderLabel.FontFace = FontBold
    configHeaderLabel.TextSize = 13
    configHeaderLabel.TextColor3 = palette.AccentBright
    configHeaderLabel.TextXAlignment = Enum.TextXAlignment.Left
    configHeaderLabel.Text = "Settings"
    configHeaderLabel.LayoutOrder = 0
    configHeaderLabel.ZIndex = 201
    configHeaderLabel.Parent = configDrawer
    bindThemeProp(configHeaderLabel, "TextColor3", "AccentBright")
    local configHeaderDivider = Instance.new("Frame")
    configHeaderDivider.BackgroundColor3 = palette.Border
    configHeaderDivider.BackgroundTransparency = 0.6
    configHeaderDivider.Size = UDim2.new(1, 0, 0, 1)
    configHeaderDivider.LayoutOrder = 1
    configHeaderDivider.BorderSizePixel = 0
    configHeaderDivider.ZIndex = 201
    configHeaderDivider.Parent = configDrawer
    bindThemeProp(configHeaderDivider, "BackgroundColor3", "Border")
    local saveUISettings = nil
    local defaultAcrylicOpacity = 0.55
    local opacityCardFrame = Instance.new("Frame")
    opacityCardFrame.BackgroundColor3 = palette.Background
    opacityCardFrame.BackgroundTransparency = 0.85
    opacityCardFrame.Size = UDim2.new(1, 0, 0, 0)
    opacityCardFrame.AutomaticSize = Enum.AutomaticSize.Y
    opacityCardFrame.LayoutOrder = 2
    opacityCardFrame.ZIndex = 201
    opacityCardFrame.Parent = configDrawer
    addCorner(opacityCardFrame, 6)
    addPadding(opacityCardFrame, 10, 12, 12, 12)
    bindThemeProp(opacityCardFrame, "BackgroundColor3", "Background")
    local opacityCardLayout = Instance.new("UIListLayout")
    opacityCardLayout.FillDirection = Enum.FillDirection.Vertical
    opacityCardLayout.Padding = UDim.new(0, 8)
    opacityCardLayout.SortOrder = Enum.SortOrder.LayoutOrder
    opacityCardLayout.Parent = opacityCardFrame
    local opacityHeaderRow = Instance.new("Frame")
    opacityHeaderRow.BackgroundTransparency = 1
    opacityHeaderRow.Size = UDim2.new(1, 0, 0, 18)
    opacityHeaderRow.LayoutOrder = 1
    opacityHeaderRow.ZIndex = 202
    opacityHeaderRow.Parent = opacityCardFrame
    local opacityTitleLabel = Instance.new("TextLabel")
    opacityTitleLabel.BackgroundTransparency = 1
    opacityTitleLabel.Size = UDim2.new(1, -52, 1, 0)
    opacityTitleLabel.FontFace = FontBold
    opacityTitleLabel.TextSize = 11
    opacityTitleLabel.TextColor3 = palette.TextWhite
    opacityTitleLabel.TextTransparency = 0
    opacityTitleLabel.TextXAlignment = Enum.TextXAlignment.Left
    opacityTitleLabel.Text = "Opacity"
    opacityTitleLabel.ZIndex = 203
    opacityTitleLabel.Parent = opacityHeaderRow
    bindThemeProp(opacityTitleLabel, "TextColor3", "TextWhite")
    local opacityInputBox = Instance.new("TextBox")
    opacityInputBox.BackgroundColor3 = Color3.fromRGB(28, 28, 28)
    opacityInputBox.BackgroundTransparency = 0.3
    opacityInputBox.Size = UDim2.new(0, 42, 0, 18)
    opacityInputBox.Position = UDim2.new(1, -42, 0.5, -9)
    opacityInputBox.FontFace = FontMedium
    opacityInputBox.TextSize = 11
    opacityInputBox.TextColor3 = palette.TextWhite
    opacityInputBox.TextTransparency = 0
    opacityInputBox.Text = tostring(math.floor(defaultAcrylicOpacity * 100)) .. "%"
    opacityInputBox.ClearTextOnFocus = false
    opacityInputBox.ZIndex = 203
    opacityInputBox.Parent = opacityHeaderRow
    addCorner(opacityInputBox, 5)
    bindThemeProp(opacityInputBox, "TextColor3", "TextWhite")
    local opacitySliderContainer = Instance.new("Frame")
    opacitySliderContainer.BackgroundTransparency = 1
    opacitySliderContainer.Size = UDim2.new(1, 0, 0, 12)
    opacitySliderContainer.LayoutOrder = 2
    opacitySliderContainer.ZIndex = 202
    opacitySliderContainer.Parent = opacityCardFrame
    local opacitySliderTrack = Instance.new("Frame")
    opacitySliderTrack.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
    opacitySliderTrack.BackgroundTransparency = 0.2
    opacitySliderTrack.Size = UDim2.new(1, 0, 0, 4)
    opacitySliderTrack.Position = UDim2.new(0, 0, 0.5, -2)
    opacitySliderTrack.ZIndex = 203
    opacitySliderTrack.Parent = opacitySliderContainer
    addCorner(opacitySliderTrack, 2)
    local opacitySliderFill = Instance.new("Frame")
    opacitySliderFill.BackgroundColor3 = palette.Accent
    opacitySliderFill.BackgroundTransparency = 0.2
    opacitySliderFill.Size = UDim2.new(defaultAcrylicOpacity, 0, 1, 0)
    opacitySliderFill.ZIndex = 204
    opacitySliderFill.Parent = opacitySliderTrack
    addCorner(opacitySliderFill, 2)
    onThemeChange(function()
        opacitySliderFill.BackgroundColor3 = palette.Accent
    end)
    local opacitySliderKnob = Instance.new("Frame")
    opacitySliderKnob.BackgroundColor3 = palette.TextWhite
    opacitySliderKnob.BackgroundTransparency = 0.2
    opacitySliderKnob.Size = UDim2.new(0, 12, 0, 12)
    opacitySliderKnob.Position = UDim2.new(defaultAcrylicOpacity, -6, 0.5, -6)
    opacitySliderKnob.ZIndex = 205
    opacitySliderKnob.Parent = opacitySliderTrack
    addCorner(opacitySliderKnob, 6)
    local opacitySliderHitBtn = Instance.new("TextButton")
    opacitySliderHitBtn.BackgroundTransparency = 1
    opacitySliderHitBtn.Size = UDim2.new(1, 0, 1, 0)
    opacitySliderHitBtn.Text = ""
    opacitySliderHitBtn.ZIndex = 206
    opacitySliderHitBtn.AutoButtonColor = false
    opacitySliderHitBtn.Parent = opacitySliderContainer
    opacityCardFrame.InputBegan:Connect(function(c0)
        if c0.UserInputType == Enum.UserInputType.MouseMovement then
            cancelGroupTweens("ophov")
            playGroupTween("ophov", opacityCardFrame, TweenInfo020, {
                BackgroundTransparency = 0.5,
            })
        end
    end)
    opacityCardFrame.InputEnded:Connect(function(c0)
        if c0.UserInputType == Enum.UserInputType.MouseMovement then
            cancelGroupTweens("ophov")
            playGroupTween("ophov", opacityCardFrame, TweenInfo020, {
                BackgroundTransparency = 0.85,
            })
        end
    end)
    local syncOpacityVisuals = function()
        opacityInputBox.Text = tostring(math.floor(winState.acrylicOpacity * 100)) .. "%"
        mainFrame.BackgroundTransparency = (winState.acrylicEnabled and winState.acrylicOpacity) or 0
    end
    local isDraggingOpacity = false
    opacityInputBox.FocusLost:Connect(function()
        local c0 = tonumber(opacityInputBox.Text:match("%d+"))
        if c0 then
            local c1 = math.clamp(c0, 0, 100) / 100
            winState.acrylicOpacity = c1
            opacitySliderFill.Size = UDim2.new(c1, 0, 1, 0)
            opacitySliderKnob.Position = UDim2.new(c1, -6, 0.5, -6)
            syncOpacityVisuals()
        else
            syncOpacityVisuals()
        end
    end)
    opacitySliderHitBtn.InputBegan:Connect(function(c0)
        if (c0.UserInputType == Enum.UserInputType.MouseButton1) or (c0.UserInputType == Enum.UserInputType.Touch) then
            isDraggingOpacity = true
            local c1 = math.clamp((c0.Position.X - opacitySliderTrack.AbsolutePosition.X) / opacitySliderTrack.AbsoluteSize.X, 0, 1)
            winState.acrylicOpacity = c1
            opacitySliderFill.Size = UDim2.new(c1, 0, 1, 0)
            opacitySliderKnob.Position = UDim2.new(c1, -6, 0.5, -6)
            syncOpacityVisuals()
        end
    end)
    table.insert(winState.connections, UserInputService.InputChanged:Connect(function(c0)
        if isDraggingOpacity and ((c0.UserInputType == Enum.UserInputType.MouseMovement) or (c0.UserInputType == Enum.UserInputType.Touch)) then
            local c1 = math.clamp((c0.Position.X - opacitySliderTrack.AbsolutePosition.X) / opacitySliderTrack.AbsoluteSize.X, 0, 1)
            winState.acrylicOpacity = c1
            opacitySliderFill.Size = UDim2.new(c1, 0, 1, 0)
            opacitySliderKnob.Position = UDim2.new(c1, -6, 0.5, -6)
            syncOpacityVisuals()
        end
    end))
    table.insert(winState.connections, UserInputService.InputEnded:Connect(function(c0)
        if (c0.UserInputType == Enum.UserInputType.MouseButton1) or (c0.UserInputType == Enum.UserInputType.Touch) then
            isDraggingOpacity = false
        end
    end))
    local acrylicRowFrame = Instance.new("Frame")
    acrylicRowFrame.BackgroundColor3 = palette.Background
    acrylicRowFrame.BackgroundTransparency = 0.85
    acrylicRowFrame.Size = UDim2.new(1, 0, 0, 34)
    acrylicRowFrame.LayoutOrder = 3
    acrylicRowFrame.ZIndex = 201
    acrylicRowFrame.Parent = configDrawer
    addCorner(acrylicRowFrame, 6)
    bindThemeProp(acrylicRowFrame, "BackgroundColor3", "Background")
    local acrylicTitleLabel = Instance.new("TextLabel")
    acrylicTitleLabel.BackgroundTransparency = 1
    acrylicTitleLabel.Size = UDim2.new(1, -60, 0, 18)
    acrylicTitleLabel.Position = UDim2.new(0, 6, 0.5, -9)
    acrylicTitleLabel.FontFace = FontBold
    acrylicTitleLabel.TextSize = 11
    acrylicTitleLabel.TextColor3 = palette.TextWhite
    acrylicTitleLabel.TextTransparency = 0.15
    acrylicTitleLabel.TextXAlignment = Enum.TextXAlignment.Left
    acrylicTitleLabel.Text = "Acrylic"
    acrylicTitleLabel.ZIndex = 202
    acrylicTitleLabel.Parent = acrylicRowFrame
    bindThemeProp(acrylicTitleLabel, "TextColor3", "TextWhite")
    local acrylicToggleBtn = Instance.new("TextButton")
    acrylicToggleBtn.Size = UDim2.new(0, 44, 0, 22)
    acrylicToggleBtn.Position = UDim2.new(1, -50, 0.5, -11)
    acrylicToggleBtn.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
    acrylicToggleBtn.BackgroundTransparency = 0.2
    acrylicToggleBtn.Text = ""
    acrylicToggleBtn.AutoButtonColor = false
    acrylicToggleBtn.ZIndex = 202
    acrylicToggleBtn.Parent = acrylicRowFrame
    addCorner(acrylicToggleBtn, 11)
    local acrylicToggleKnob = Instance.new("Frame")
    acrylicToggleKnob.BackgroundColor3 = Color3.fromRGB(235, 235, 235)
    acrylicToggleKnob.BackgroundTransparency = 0.2
    acrylicToggleKnob.Size = UDim2.new(0, 16, 0, 16)
    acrylicToggleKnob.Position = UDim2.new(0, 3, 0.5, -8)
    acrylicToggleKnob.ZIndex = 203
    acrylicToggleKnob.Parent = acrylicToggleBtn
    addCorner(acrylicToggleKnob, 8)
    onThemeChange(function()
        if winState.acrylicEnabled then
            acrylicToggleBtn.BackgroundColor3 = palette.Accent
        end
    end)
    acrylicRowFrame.InputBegan:Connect(function(c0)
        if c0.UserInputType == Enum.UserInputType.MouseMovement then
            cancelGroupTweens("acrhov")
            playGroupTween("acrhov", acrylicToggleBtn, TweenInfo020, {
                BackgroundTransparency = 0,
            })
            playGroupTween("acrhov", acrylicToggleKnob, TweenInfo020, {
                BackgroundTransparency = 0,
            })
            playGroupTween("acrhov", acrylicRowFrame, TweenInfo020, {
                BackgroundTransparency = 0.5,
            })
        end
    end)
    acrylicRowFrame.InputEnded:Connect(function(c0)
        if c0.UserInputType == Enum.UserInputType.MouseMovement then
            cancelGroupTweens("acrhov")
            playGroupTween("acrhov", acrylicToggleBtn, TweenInfo020, {
                BackgroundTransparency = 0.2,
            })
            playGroupTween("acrhov", acrylicToggleKnob, TweenInfo020, {
                BackgroundTransparency = 0.2,
            })
            playGroupTween("acrhov", acrylicRowFrame, TweenInfo020, {
                BackgroundTransparency = 0.85,
            })
        end
    end)
    table.insert(winState.connections, acrylicToggleBtn.MouseButton1Click:Connect(function()
        if winState.destroyed then
            return
        end
        playSound(SOUND_OPEN)
        winState.acrylicEnabled = not winState.acrylicEnabled
        local c0 = winState.acrylicEnabled
        cancelGroupTweens("acrylic_toggle")
        playGroupTween("acrylic_toggle", acrylicToggleBtn, TweenInfo020, {
            BackgroundColor3 = (c0 and palette.Accent) or Color3.fromRGB(50, 50, 50),
        })
        playGroupTween("acrylic_toggle", acrylicToggleKnob, TweenInfo020, {
            Position = (c0 and UDim2.new(1, -19, 0.5, -8)) or UDim2.new(0, 3, 0.5, -8),
        })
        playGroupTween("acrylic_toggle", mainFrame, TweenInfo035, {
            BackgroundTransparency = (c0 and winState.acrylicOpacity) or 0,
        })
        saveUISettings()
    end))
    local drawerHintLabel = Instance.new("TextLabel")
    drawerHintLabel.BackgroundTransparency = 1
    drawerHintLabel.Size = UDim2.new(1, 0, 0, 20)
    drawerHintLabel.FontFace = FontRegular
    drawerHintLabel.TextSize = 9
    drawerHintLabel.TextColor3 = palette.TextWhite
    drawerHintLabel.TextTransparency = 0.7
    drawerHintLabel.Text = "Click outside to close"
    drawerHintLabel.LayoutOrder = 9999
    drawerHintLabel.ZIndex = 201
    drawerHintLabel.Parent = configDrawer
    bindThemeProp(drawerHintLabel, "TextColor3", "TextWhite")
    local drawerDividerLine = Instance.new("Frame")
    drawerDividerLine.BackgroundColor3 = palette.Border
    drawerDividerLine.BackgroundTransparency = 0.6
    drawerDividerLine.Size = UDim2.new(1, 0, 0, 1)
    drawerDividerLine.LayoutOrder = 4
    drawerDividerLine.BorderSizePixel = 0
    drawerDividerLine.ZIndex = 201
    drawerDividerLine.Parent = configDrawer
    bindThemeProp(drawerDividerLine, "BackgroundColor3", "Border")
    local currentThemeName = ((typeof(windowOpts.Theme) == "Color3") and "Custom") or (windowOpts.Theme or "Red")
    local settingsFolder = "VexzHub"
    local uiSettingsPath = settingsFolder .. "/UISettings.json"
    pcall(function()
        if makefolder and (not isfolder(settingsFolder)) then
            makefolder(settingsFolder)
        end
    end)
    local uiSettings = {}
    uiSettings.showFps = true
    uiSettings.showPing = false
    uiSettings.showProfile = true
    uiSettings.theme = currentThemeName
    uiSettings.acrylicEnabled = false
    uiSettings.acrylicOpacity = 0.55
    uiSettings.wallpaperOpacity = 0.75
    uiSettings.backgroundImageId = ""
    uiSettings.customColorHex = ""
    saveUISettings = function()
        pcall(function()
            writefile(uiSettingsPath, game:GetService("HttpService"):JSONEncode({
                showFps = showFps,
                showPing = showPing,
                showProfile = showProfile,
                theme = currentThemeName,
                acrylicEnabled = winState.acrylicEnabled,
                acrylicOpacity = winState.acrylicOpacity,
                wallpaperOpacity = winState.wallpaperOpacity,
                backgroundImageId = winState.backgroundImageId,
                customColorHex = winState.customColorHex,
            }))
        end)
    end
    local loadUISettings = function()
        local c0, c1 = pcall(function()
            if not isfile(uiSettingsPath) then
                return
            end
            local d1 = game:GetService("HttpService"):JSONDecode(readfile(uiSettingsPath))
            if type(d1) == "table" then
                if type(d1.showFps) == "boolean" then
                    uiSettings.showFps = d1.showFps
                end
                if type(d1.showPing) == "boolean" then
                    uiSettings.showPing = d1.showPing
                end
                if type(d1.showProfile) == "boolean" then
                    uiSettings.showProfile = d1.showProfile
                end
                if type(d1.theme) == "string" then
                    uiSettings.theme = d1.theme
                end
                if type(d1.acrylicEnabled) == "boolean" then
                    uiSettings.acrylicEnabled = d1.acrylicEnabled
                end
                if type(d1.acrylicOpacity) == "number" then
                    uiSettings.acrylicOpacity = d1.acrylicOpacity
                end
                if type(d1.wallpaperOpacity) == "number" then
                    uiSettings.wallpaperOpacity = d1.wallpaperOpacity
                end
                if type(d1.backgroundImageId) == "string" then
                    uiSettings.backgroundImageId = d1.backgroundImageId
                end
                if type(d1.customColorHex) == "string" then
                    uiSettings.customColorHex = d1.customColorHex
                end
            end
        end)
    end
    loadUISettings()
    local configDrawerStrokeRef = configDrawerStroke
    local themePickerOpen = false
    local themeHexLabel = nil
    local themePreviewSwatch = nil
    local closeConfigDrawer = nil
    local applyThemePalette = function(c0)
        currentThemeName = ((typeof(c0) == "Color3") and "Custom") or tostring(c0)
        if typeof(c0) == "Color3" then
            for c5, c6 in pairs(buildPaletteFromColor(c0)) do
                palette[c5] = boostColorHSV(c6, 0.45)
            end
        else
            for c4, c5 in pairs(ColorPresets[c0] or ColorPresets.Red) do
                palette[c4] = boostColorHSV(c5, 0.45)
            end
        end
        mainFrame.BackgroundColor3 = palette.Background
        configDrawer.BackgroundColor3 = palette.ConfigPanel
        sidebarDivider.BackgroundColor3 = palette.Border
        headerFrame.BackgroundColor3 = palette.Border
        opacitySliderFill.BackgroundColor3 = palette.Accent
        configHeaderLabel.TextColor3 = palette.AccentBright
        fpsLabel.TextColor3 = palette.AccentBright
        pingLabel.TextColor3 = palette.AccentBright
        if configDrawerStrokeRef then
            configDrawerStrokeRef.Color = palette.Border
        end
        for c4, c5 in ipairs(configCardStrokes) do
            c5.BackgroundColor3 = palette.Accent
        end
        headerBtnIcons.Config.ImageColor3 = palette.AccentDeep
        headerBtnIcons.Minimize.ImageColor3 = palette.AccentDark
        headerBtnIcons.Maximize.ImageColor3 = palette.Accent
        headerBtnIcons.Close.ImageColor3 = palette.Accent
        for c4, c5 in pairs(winState.tabs) do
            c5.indicator.BackgroundColor3 = palette.Accent
            if winState.selectedTab == c4 then
                c5.titleLabel.TextColor3 = palette.AccentBright
                c5.subtitleLabel.TextColor3 = palette.Accent
                c5.iconLabel.ImageColor3 = palette.AccentBright
                c5.frame.BackgroundColor3 = palette.TabSelected
            end
        end
        for c4, c5 in ipairs(winState.themeCallbacks) do
            pcall(c5)
        end
        for c4, c5 in ipairs(winState.accentElems) do
            pcall(function()
                c5.inst[c5.prop] = palette[c5.key]
            end)
        end
        if themeHexLabel then
            themeHexLabel.Text = string.format("#%02X%02X%02X", math.floor((palette.Accent.R * 255) + 0.5), math.floor((palette.Accent.G * 255) + 0.5), math.floor((palette.Accent.B * 255) + 0.5))
        end
        if themePreviewSwatch then
            themePreviewSwatch.BackgroundColor3 = palette.Accent
        end
    end
    local selectAndSaveTheme = function(c0)
        if closeConfigDrawer then
            closeConfigDrawer()
        end
        cancelGroupTweens("theme_anim")
        local c1 = TweenInfo.new(0.22, Enum.EasingStyle.Quart, Enum.EasingDirection.In)
        playGroupTween("theme_anim", mainFrame, c1, {
            BackgroundTransparency = 1,
        })
        playGroupTween("theme_anim", mainStroke, c1, {
            Transparency = 1,
        })
        local c2 = mainFrame:FindFirstChild("Shadow")
        if c2 then
            playGroupTween("theme_anim", c2, c1, {
                ImageTransparency = 1,
            })
        end
        task.delay(0.26, function()
            mainFrame.Visible = false
            applyThemePalette(c0)
            if wallpaperImage then
                if winState.backgroundImageId and (winState.backgroundImageId ~= "") then
                    wallpaperImage.Image = "rbxassetid://" .. winState.backgroundImageId
                    wallpaperImage.Visible = true
                else
                    wallpaperImage.Visible = false
                end
                wallpaperImage.ImageTransparency = 1 - winState.wallpaperOpacity
            end
            saveUISettings()
            playLoadingScreen(palette, function()
                mainFrame.Visible = true
                cancelGroupTweens("theme_anim")
                playGroupTween("theme_anim", mainFrame, TweenInfo045, {
                    BackgroundTransparency = (winState.acrylicEnabled and winState.acrylicOpacity) or 0,
                })
                playGroupTween("theme_anim", mainStroke, TweenInfo045, {
                    Transparency = 0.6,
                })
                local e0 = mainFrame:FindFirstChild("Shadow")
                if e0 then
                    playGroupTween("theme_anim", e0, TweenInfo060, {
                        ImageTransparency = 0.5,
                    })
                end
            end)
        end)
    end
    local themeCardFrame = Instance.new("Frame")
    themeCardFrame.BackgroundTransparency = 1
    themeCardFrame.Size = UDim2.new(1, 0, 0, 0)
    themeCardFrame.AutomaticSize = Enum.AutomaticSize.Y
    themeCardFrame.LayoutOrder = 6
    themeCardFrame.ZIndex = 201
    themeCardFrame.Parent = configDrawer
    local themeCardLayout = Instance.new("UIListLayout")
    themeCardLayout.FillDirection = Enum.FillDirection.Vertical
    themeCardLayout.Padding = UDim.new(0, 4)
    themeCardLayout.SortOrder = Enum.SortOrder.LayoutOrder
    themeCardLayout.Parent = themeCardFrame
    local themeDropdownHeader = Instance.new("Frame")
    themeDropdownHeader.BackgroundColor3 = palette.Background
    themeDropdownHeader.BackgroundTransparency = 0.85
    themeDropdownHeader.Size = UDim2.new(1, 0, 0, 40)
    themeDropdownHeader.LayoutOrder = 1
    themeDropdownHeader.ZIndex = 202
    themeDropdownHeader.Parent = themeCardFrame
    addCorner(themeDropdownHeader, 6)
    addPadding(themeDropdownHeader, 6, 12, 6, 12)
    bindThemeProp(themeDropdownHeader, "BackgroundColor3", "Background")
    local themeHeaderStroke = Instance.new("UIStroke")
    themeHeaderStroke.Color = palette.Accent
    themeHeaderStroke.Thickness = 1
    themeHeaderStroke.Transparency = 1
    themeHeaderStroke.Parent = themeDropdownHeader
    onThemeChange(function()
        themeHeaderStroke.Color = palette.Accent
    end)
    themeDropdownHeader.InputBegan:Connect(function(c0)
        if c0.UserInputType == Enum.UserInputType.MouseMovement then
            themeHeaderStroke.Color = palette.Accent
            cancelGroupTweens("thdrophov_glow")
            playGroupTween("thdrophov_glow", themeHeaderStroke, TweenInfo020, {
                Transparency = 0.55,
            })
        end
    end)
    themeDropdownHeader.InputEnded:Connect(function(c0)
        if c0.UserInputType == Enum.UserInputType.MouseMovement then
            cancelGroupTweens("thdrophov_glow")
            playGroupTween("thdrophov_glow", themeHeaderStroke, TweenInfo020, {
                Transparency = 1,
            })
        end
    end)
    local themeHeaderContent = Instance.new("Frame")
    themeHeaderContent.BackgroundTransparency = 1
    themeHeaderContent.Size = UDim2.new(1, 0, 1, 0)
    themeHeaderContent.ZIndex = 202
    themeHeaderContent.Parent = themeDropdownHeader
    local themeHeaderTitle = Instance.new("TextLabel")
    themeHeaderTitle.BackgroundTransparency = 1
    themeHeaderTitle.Size = UDim2.new(1, -34, 0, 16)
    themeHeaderTitle.Position = UDim2.new(0, 0, 0, 0)
    themeHeaderTitle.FontFace = FontBold
    themeHeaderTitle.TextSize = 11
    themeHeaderTitle.TextColor3 = palette.TextWhite
    themeHeaderTitle.TextXAlignment = Enum.TextXAlignment.Left
    themeHeaderTitle.Text = "Theme Color"
    themeHeaderTitle.ZIndex = 203
    themeHeaderTitle.Parent = themeHeaderContent
    bindThemeProp(themeHeaderTitle, "TextColor3", "TextWhite")
    themeHexLabel = Instance.new("TextLabel")
    themeHexLabel.BackgroundTransparency = 1
    themeHexLabel.Size = UDim2.new(1, -34, 0, 12)
    themeHexLabel.Position = UDim2.new(0, 0, 0, 16)
    themeHexLabel.FontFace = FontMedium
    themeHexLabel.TextSize = 10
    themeHexLabel.TextColor3 = palette.TextSubtitle
    themeHexLabel.TextXAlignment = Enum.TextXAlignment.Left
    themeHexLabel.Text = string.format("#%02X%02X%02X", math.floor((palette.Accent.R * 255) + 0.5), math.floor((palette.Accent.G * 255) + 0.5), math.floor((palette.Accent.B * 255) + 0.5))
    themeHexLabel.ZIndex = 203
    themeHexLabel.Parent = themeHeaderContent
    bindThemeProp(themeHexLabel, "TextColor3", "TextSubtitle")
    themePreviewSwatch = Instance.new("Frame")
    themePreviewSwatch.BackgroundColor3 = palette.Accent
    themePreviewSwatch.Size = UDim2.new(0, 26, 0, 26)
    themePreviewSwatch.AnchorPoint = Vector2.new(1, 0.5)
    themePreviewSwatch.Position = UDim2.new(1, 0, 0.5, 0)
    themePreviewSwatch.ZIndex = 203
    themePreviewSwatch.Parent = themeHeaderContent
    addCorner(themePreviewSwatch, 6)
    local themeSwatchStroke = addStroke(themePreviewSwatch, palette.Border, 1, 0.3)
    onThemeChange(function()
        themeSwatchStroke.Color = palette.Border
    end)
    local pickerDrawerFrame = Instance.new("Frame")
    pickerDrawerFrame.BackgroundTransparency = 1
    pickerDrawerFrame.Size = UDim2.new(1, 0, 0, 0)
    pickerDrawerFrame.ClipsDescendants = true
    pickerDrawerFrame.LayoutOrder = 2
    pickerDrawerFrame.ZIndex = 202
    pickerDrawerFrame.Parent = themeCardFrame
    local colorPickerBox = Instance.new("Frame")
    colorPickerBox.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
    colorPickerBox.Size = UDim2.new(1, 0, 0, 0)
    colorPickerBox.AutomaticSize = Enum.AutomaticSize.Y
    colorPickerBox.ZIndex = 202
    colorPickerBox.Parent = pickerDrawerFrame
    addCorner(colorPickerBox, 8)
    local colorPickerStroke = addStroke(colorPickerBox, palette.Border, 1, 0.45)
    onThemeChange(function()
        colorPickerStroke.Color = palette.Border
    end)
    local colorPickerLayout = Instance.new("UIListLayout")
    colorPickerLayout.FillDirection = Enum.FillDirection.Vertical
    colorPickerLayout.Padding = UDim.new(0, 4)
    colorPickerLayout.SortOrder = Enum.SortOrder.LayoutOrder
    colorPickerLayout.Parent = colorPickerBox
    addPadding(colorPickerBox, 5, 5, 5, 5)
    local pickerPanelHeight = 240
    local curHue, curSat, curVal = palette.Accent:ToHSV()
    local svSquareFrame = Instance.new("Frame")
    svSquareFrame.BackgroundColor3 = Color3.fromHSV(curHue, 1, 1)
    svSquareFrame.Size = UDim2.new(1, 0, 0, 120)
    svSquareFrame.LayoutOrder = 1
    svSquareFrame.ClipsDescendants = true
    svSquareFrame.ZIndex = 203
    svSquareFrame.Parent = colorPickerBox
    addCorner(svSquareFrame, 6)
    local satGradientOverlay = Instance.new("Frame")
    satGradientOverlay.BackgroundColor3 = Color3.new(1, 1, 1)
    satGradientOverlay.BorderSizePixel = 0
    satGradientOverlay.Size = UDim2.new(1, 0, 1, 0)
    satGradientOverlay.ZIndex = 204
    satGradientOverlay.Parent = svSquareFrame
    local satGradient = Instance.new("UIGradient")
    satGradient.Transparency = NumberSequence.new({
        NumberSequenceKeypoint.new(0, 0),
        NumberSequenceKeypoint.new(1, 1),
    })
    satGradient.Parent = satGradientOverlay
    local valGradientOverlay = Instance.new("Frame")
    valGradientOverlay.BackgroundColor3 = Color3.new(0, 0, 0)
    valGradientOverlay.BorderSizePixel = 0
    valGradientOverlay.Size = UDim2.new(1, 0, 1, 0)
    valGradientOverlay.ZIndex = 205
    valGradientOverlay.Parent = svSquareFrame
    local valGradient = Instance.new("UIGradient")
    valGradient.Rotation = 90
    valGradient.Transparency = NumberSequence.new({
        NumberSequenceKeypoint.new(0, 1),
        NumberSequenceKeypoint.new(1, 0),
    })
    valGradient.Parent = valGradientOverlay
    local svCursorKnob = Instance.new("Frame")
    svCursorKnob.AnchorPoint = Vector2.new(0.5, 0.5)
    svCursorKnob.BackgroundColor3 = Color3.new(1, 1, 1)
    svCursorKnob.Size = UDim2.new(0, 12, 0, 12)
    svCursorKnob.Position = UDim2.new(curSat, 0, 1 - curVal, 0)
    svCursorKnob.ZIndex = 207
    svCursorKnob.Parent = svSquareFrame
    addCorner(svCursorKnob, 6)
    addStroke(svCursorKnob, Color3.new(0, 0, 0), 2, 0.2)
    local svHitButton = Instance.new("TextButton")
    svHitButton.BackgroundTransparency = 1
    svHitButton.Text = ""
    svHitButton.Size = UDim2.new(1, 0, 1, 0)
    svHitButton.AutoButtonColor = false
    svHitButton.ZIndex = 208
    svHitButton.Parent = svSquareFrame
    local hueSliderContainer = Instance.new("Frame")
    hueSliderContainer.BackgroundTransparency = 1
    hueSliderContainer.Size = UDim2.new(1, 0, 0, 18)
    hueSliderContainer.LayoutOrder = 2
    hueSliderContainer.ZIndex = 203
    hueSliderContainer.Parent = colorPickerBox
    local hueTrackBar = Instance.new("Frame")
    hueTrackBar.BackgroundColor3 = Color3.new(1, 1, 1)
    hueTrackBar.BorderSizePixel = 0
    hueTrackBar.Size = UDim2.new(1, 0, 0, 8)
    hueTrackBar.Position = UDim2.new(0, 0, 0.5, -4)
    hueTrackBar.ZIndex = 203
    hueTrackBar.Parent = hueSliderContainer
    addCorner(hueTrackBar, 4)
    local hueGradient = Instance.new("UIGradient")
    hueGradient.Color = ColorSequence.new({
        ColorSequenceKeypoint.new(0, Color3.fromHSV(0, 1, 1)),
        ColorSequenceKeypoint.new(1 / 6, Color3.fromHSV(1 / 6, 1, 1)),
        ColorSequenceKeypoint.new(2 / 6, Color3.fromHSV(2 / 6, 1, 1)),
        ColorSequenceKeypoint.new(3 / 6, Color3.fromHSV(3 / 6, 1, 1)),
        ColorSequenceKeypoint.new(4 / 6, Color3.fromHSV(4 / 6, 1, 1)),
        ColorSequenceKeypoint.new(5 / 6, Color3.fromHSV(5 / 6, 1, 1)),
        ColorSequenceKeypoint.new(1, Color3.fromHSV(1, 1, 1)),
    })
    hueGradient.Parent = hueTrackBar
    local hueCursorKnob = Instance.new("Frame")
    hueCursorKnob.AnchorPoint = Vector2.new(0.5, 0.5)
    hueCursorKnob.BackgroundColor3 = Color3.new(1, 1, 1)
    hueCursorKnob.Size = UDim2.new(0, 14, 0, 14)
    hueCursorKnob.Position = UDim2.new(curHue, 0, 0.5, 0)
    hueCursorKnob.ZIndex = 205
    hueCursorKnob.Parent = hueSliderContainer
    addCorner(hueCursorKnob, 7)
    addStroke(hueCursorKnob, Color3.new(0, 0, 0), 2, 0.2)
    local hueInputButton = Instance.new("TextButton")
    hueInputButton.BackgroundTransparency = 1
    hueInputButton.Text = ""
    hueInputButton.Size = UDim2.new(1, 0, 1, 0)
    hueInputButton.AutoButtonColor = false
    hueInputButton.ZIndex = 206
    hueInputButton.Parent = hueSliderContainer
    local colorInputsContainer = Instance.new("Frame")
    colorInputsContainer.BackgroundTransparency = 1
    colorInputsContainer.Size = UDim2.new(1, 0, 0, 50)
    colorInputsContainer.LayoutOrder = 3
    colorInputsContainer.ZIndex = 203
    colorInputsContainer.Parent = colorPickerBox
    local colorInputsLayout = Instance.new("UIListLayout")
    colorInputsLayout.Padding = UDim.new(0, 2)
    colorInputsLayout.SortOrder = Enum.SortOrder.LayoutOrder
    colorInputsLayout.Parent = colorInputsContainer
    local createColorInputRow = function(c0, c1)
        local c2 = Instance.new("Frame")
        c2.BackgroundTransparency = 1
        c2.Size = UDim2.new(1, 0, 0, 14)
        c2.LayoutOrder = c0
        c2.ZIndex = 203
        c2.Parent = colorInputsContainer
        local c3 = Instance.new("TextLabel")
        c3.BackgroundTransparency = 1
        c3.Size = UDim2.new(0, 36, 1, 0)
        c3.FontFace = FontBold
        c3.TextSize = 10
        c3.TextColor3 = palette.TextSubtitle
        c3.TextXAlignment = Enum.TextXAlignment.Left
        c3.Text = c1
        c3.ZIndex = 203
        c3.Parent = c2
        bindThemeProp(c3, "TextColor3", "TextSubtitle")
        local c4 = Instance.new("TextLabel")
        c4.BackgroundTransparency = 1
        c4.Size = UDim2.new(1, -36, 1, 0)
        c4.Position = UDim2.new(0, 36, 0, 0)
        c4.FontFace = FontMedium
        c4.TextSize = 10
        c4.TextColor3 = palette.TextWhite
        c4.TextXAlignment = Enum.TextXAlignment.Left
        c4.ZIndex = 203
        c4.Parent = c2
        bindThemeProp(c4, "TextColor3", "TextWhite")
        return c4
    end
    local hexInputBox = createColorInputRow(1, "Hex")
    local rgbInputBox = createColorInputRow(2, "RGB")
    local hslInputBox = createColorInputRow(3, "HSL")
    local applyCustomColorBtn = Instance.new("TextButton")
    applyCustomColorBtn.BackgroundColor3 = palette.Accent
    applyCustomColorBtn.Size = UDim2.new(1, 0, 0, 26)
    applyCustomColorBtn.LayoutOrder = 4
    applyCustomColorBtn.FontFace = FontBold
    applyCustomColorBtn.TextSize = 11
    applyCustomColorBtn.TextColor3 = Color3.new(1, 1, 1)
    applyCustomColorBtn.Text = "Apply"
    applyCustomColorBtn.AutoButtonColor = false
    applyCustomColorBtn.ZIndex = 203
    applyCustomColorBtn.Parent = colorPickerBox
    addCorner(applyCustomColorBtn, 5)
    onThemeChange(function()
        applyCustomColorBtn.BackgroundColor3 = palette.Accent
    end)
    local rgbToHslPercent = function(c0, c1, c2)
        local c3 = math.max(c0, c1, c2)
        local c4 = math.min(c0, c1, c2)
        local c5 = 0
        local c6 = 0
        local c7 = (c3 + c4) / 2
        local c8 = c3 - c4
        if c8 ~= 0 then
            c6 = ((c7 > 0.5) and (c8 / ((2 - c3) - c4))) or (c8 / (c3 + c4))
            if c3 == c0 then
                c5 = ((c1 - c2) / c8) % 6
            elseif c3 == c1 then
                c5 = ((c2 - c0) / c8) + 2
            else
                c5 = ((c0 - c1) / c8) + 4
            end
            c5 = c5 / 6
        end
        return math.floor((c5 * 360) + 0.5), math.floor((c6 * 100) + 0.5), math.floor((c7 * 100) + 0.5)
    end
    local updateColorPickerVisuals = function()
        svSquareFrame.BackgroundColor3 = Color3.fromHSV(curHue, 1, 1)
        svCursorKnob.Position = UDim2.new(curSat, 0, 1 - curVal, 0)
        hueCursorKnob.Position = UDim2.new(curHue, 0, 0.5, 0)
        local c1 = Color3.fromHSV(curHue, curSat, curVal)
        local c2 = math.floor((c1.R * 255) + 0.5)
        local c3 = math.floor((c1.G * 255) + 0.5)
        local c4 = math.floor((c1.B * 255) + 0.5)
        hexInputBox.Text = string.format("#%02X%02X%02X", c2, c3, c4)
        rgbInputBox.Text = c2 .. ", " .. c3 .. ", " .. c4
        local c5, c6, c7 = rgbToHslPercent(c1.R, c1.G, c1.B)
        hslInputBox.Text = c5 .. ", " .. c6 .. ", " .. c7
    end
    updateColorPickerVisuals()
    local isDraggingSV = false
    svHitButton.InputBegan:Connect(function(c0)
        if (c0.UserInputType == Enum.UserInputType.MouseButton1) or (c0.UserInputType == Enum.UserInputType.Touch) then
            isDraggingSV = true
            curSat = math.clamp((c0.Position.X - svSquareFrame.AbsolutePosition.X) / svSquareFrame.AbsoluteSize.X, 0, 1)
            curVal = 1 - math.clamp((c0.Position.Y - svSquareFrame.AbsolutePosition.Y) / svSquareFrame.AbsoluteSize.Y, 0, 1)
            updateColorPickerVisuals()
        end
    end)
    table.insert(winState.connections, UserInputService.InputChanged:Connect(function(c0)
        if isDraggingSV and ((c0.UserInputType == Enum.UserInputType.MouseMovement) or (c0.UserInputType == Enum.UserInputType.Touch)) then
            curSat = math.clamp((c0.Position.X - svSquareFrame.AbsolutePosition.X) / svSquareFrame.AbsoluteSize.X, 0, 1)
            curVal = 1 - math.clamp((c0.Position.Y - svSquareFrame.AbsolutePosition.Y) / svSquareFrame.AbsoluteSize.Y, 0, 1)
            updateColorPickerVisuals()
        end
    end))
    table.insert(winState.connections, UserInputService.InputEnded:Connect(function(c0)
        if (c0.UserInputType == Enum.UserInputType.MouseButton1) or (c0.UserInputType == Enum.UserInputType.Touch) then
            isDraggingSV = false
        end
    end))
    local isDraggingHue = false
    hueInputButton.InputBegan:Connect(function(c0)
        if (c0.UserInputType == Enum.UserInputType.MouseButton1) or (c0.UserInputType == Enum.UserInputType.Touch) then
            isDraggingHue = true
            curHue = math.clamp((c0.Position.X - hueTrackBar.AbsolutePosition.X) / hueTrackBar.AbsoluteSize.X, 0, 1)
            updateColorPickerVisuals()
        end
    end)
    table.insert(winState.connections, UserInputService.InputChanged:Connect(function(c0)
        if isDraggingHue and ((c0.UserInputType == Enum.UserInputType.MouseMovement) or (c0.UserInputType == Enum.UserInputType.Touch)) then
            curHue = math.clamp((c0.Position.X - hueTrackBar.AbsolutePosition.X) / hueTrackBar.AbsoluteSize.X, 0, 1)
            updateColorPickerVisuals()
        end
    end))
    table.insert(winState.connections, UserInputService.InputEnded:Connect(function(c0)
        if (c0.UserInputType == Enum.UserInputType.MouseButton1) or (c0.UserInputType == Enum.UserInputType.Touch) then
            isDraggingHue = false
        end
    end))
    applyCustomColorBtn.MouseButton1Click:Connect(function()
        themePickerOpen = false
        playGroupTween("themedrop_anim", pickerDrawerFrame, TweenInfo020, {
            Size = UDim2.new(1, 0, 0, 0),
        })
        playGroupTween("themedrop_anim", themeDropdownHeader, TweenInfo020, {
            BackgroundTransparency = 0.85,
        })
        local c0 = Color3.fromHSV(curHue, curSat, curVal)
        winState.customColorHex = string.format("#%02X%02X%02X", math.floor((c0.R * 255) + 0.5), math.floor((c0.G * 255) + 0.5), math.floor((c0.B * 255) + 0.5))
        selectAndSaveTheme(c0)
    end)
    local setColorPickerFromColor = function(c0)
        local c1, c2, c3 = c0:ToHSV()
        curHue = c1
        curSat = c2
        curVal = c3
        updateColorPickerVisuals()
    end
    local themeHeaderToggleBtn = Instance.new("TextButton")
    themeHeaderToggleBtn.BackgroundTransparency = 1
    themeHeaderToggleBtn.Size = UDim2.new(1, 0, 1, 0)
    themeHeaderToggleBtn.Text = ""
    themeHeaderToggleBtn.AutoButtonColor = false
    themeHeaderToggleBtn.ZIndex = 204
    themeHeaderToggleBtn.Parent = themeDropdownHeader
    themeHeaderToggleBtn.MouseButton1Click:Connect(function()
        themePickerOpen = not themePickerOpen
        if themePickerOpen then
            cancelGroupTweens("themedrop_anim")
            playGroupTween("themedrop_anim", themeDropdownHeader, TweenInfo020, {
                BackgroundTransparency = 0.7,
            })
            playGroupTween("themedrop_anim", pickerDrawerFrame, TweenInfo035, {
                Size = UDim2.new(1, 0, 0, pickerPanelHeight),
            })
        else
            cancelGroupTweens("themedrop_anim")
            playGroupTween("themedrop_anim", themeDropdownHeader, TweenInfo020, {
                BackgroundTransparency = 0.85,
            })
            playGroupTween("themedrop_anim", pickerDrawerFrame, TweenInfo020, {
                Size = UDim2.new(1, 0, 0, 0),
            })
        end
    end)
    local wallpaperCardFrame = Instance.new("Frame")
    wallpaperCardFrame.BackgroundColor3 = palette.Background
    wallpaperCardFrame.BackgroundTransparency = 0.85
    wallpaperCardFrame.Size = UDim2.new(1, 0, 0, 144)
    wallpaperCardFrame.LayoutOrder = 7
    wallpaperCardFrame.ZIndex = 201
    wallpaperCardFrame.Parent = configDrawer
    addCorner(wallpaperCardFrame, 6)
    bindThemeProp(wallpaperCardFrame, "BackgroundColor3", "Background")
    local bgImageTitleLabel = Instance.new("TextLabel")
    bgImageTitleLabel.BackgroundTransparency = 1
    bgImageTitleLabel.Size = UDim2.new(1, -12, 0, 16)
    bgImageTitleLabel.Position = UDim2.new(0, 6, 0, 6)
    bgImageTitleLabel.FontFace = FontBold
    bgImageTitleLabel.TextSize = 11
    bgImageTitleLabel.TextColor3 = palette.TextWhite
    bgImageTitleLabel.TextXAlignment = Enum.TextXAlignment.Left
    bgImageTitleLabel.Text = "Background Image"
    bgImageTitleLabel.ZIndex = 202
    bgImageTitleLabel.Parent = wallpaperCardFrame
    bindThemeProp(bgImageTitleLabel, "TextColor3", "TextWhite")
    local bgImageInputBox = Instance.new("TextBox")
    bgImageInputBox.BackgroundColor3 = Color3.fromRGB(28, 28, 28)
    bgImageInputBox.BackgroundTransparency = 0.2
    bgImageInputBox.Size = UDim2.new(1, -12, 0, 24)
    bgImageInputBox.Position = UDim2.new(0, 6, 0, 26)
    bgImageInputBox.FontFace = FontMedium
    bgImageInputBox.TextSize = 11
    bgImageInputBox.PlaceholderText = "Enter image asset id..."
    bgImageInputBox.Text = ""
    bgImageInputBox.TextColor3 = palette.TextWhite
    bgImageInputBox.PlaceholderColor3 = palette.TextSubtitle
    bgImageInputBox.ClearTextOnFocus = false
    bgImageInputBox.ZIndex = 202
    bgImageInputBox.Parent = wallpaperCardFrame
    addCorner(bgImageInputBox, 5)
    bindThemeProp(bgImageInputBox, "TextColor3", "TextWhite")
    local wallpaperOpacityTitle = Instance.new("TextLabel")
    wallpaperOpacityTitle.BackgroundTransparency = 1
    wallpaperOpacityTitle.Size = UDim2.new(1, -54, 0, 14)
    wallpaperOpacityTitle.Position = UDim2.new(0, 6, 0, 58)
    wallpaperOpacityTitle.FontFace = FontBold
    wallpaperOpacityTitle.TextSize = 10
    wallpaperOpacityTitle.TextColor3 = palette.TextWhite
    wallpaperOpacityTitle.TextXAlignment = Enum.TextXAlignment.Left
    wallpaperOpacityTitle.Text = "Wallpaper Opacity"
    wallpaperOpacityTitle.ZIndex = 202
    wallpaperOpacityTitle.Parent = wallpaperCardFrame
    bindThemeProp(wallpaperOpacityTitle, "TextColor3", "TextWhite")
    local wallpaperOpacityBox = Instance.new("TextBox")
    wallpaperOpacityBox.BackgroundColor3 = Color3.fromRGB(28, 28, 28)
    wallpaperOpacityBox.BackgroundTransparency = 0.3
    wallpaperOpacityBox.Size = UDim2.new(0, 38, 0, 14)
    wallpaperOpacityBox.Position = UDim2.new(1, -44, 0, 58)
    wallpaperOpacityBox.FontFace = FontMedium
    wallpaperOpacityBox.TextSize = 10
    wallpaperOpacityBox.TextColor3 = palette.TextWhite
    wallpaperOpacityBox.Text = tostring(math.floor(winState.wallpaperOpacity * 100)) .. "%"
    wallpaperOpacityBox.ClearTextOnFocus = false
    wallpaperOpacityBox.ZIndex = 202
    wallpaperOpacityBox.Parent = wallpaperCardFrame
    addCorner(wallpaperOpacityBox, 4)
    bindThemeProp(wallpaperOpacityBox, "TextColor3", "TextWhite")
    local wallpaperSliderTrack = Instance.new("Frame")
    wallpaperSliderTrack.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
    wallpaperSliderTrack.BackgroundTransparency = 0.2
    wallpaperSliderTrack.Size = UDim2.new(1, -12, 0, 4)
    wallpaperSliderTrack.Position = UDim2.new(0, 6, 0, 78)
    wallpaperSliderTrack.ZIndex = 202
    wallpaperSliderTrack.Parent = wallpaperCardFrame
    addCorner(wallpaperSliderTrack, 2)
    local wallpaperSliderFill = Instance.new("Frame")
    wallpaperSliderFill.BackgroundColor3 = palette.Accent
    wallpaperSliderFill.BackgroundTransparency = 0.2
    wallpaperSliderFill.Size = UDim2.new(winState.wallpaperOpacity, 0, 1, 0)
    wallpaperSliderFill.ZIndex = 203
    wallpaperSliderFill.Parent = wallpaperSliderTrack
    addCorner(wallpaperSliderFill, 2)
    onThemeChange(function()
        wallpaperSliderFill.BackgroundColor3 = palette.Accent
    end)
    local wallpaperSliderKnob = Instance.new("Frame")
    wallpaperSliderKnob.BackgroundColor3 = palette.TextWhite
    wallpaperSliderKnob.BackgroundTransparency = 0.2
    wallpaperSliderKnob.Size = UDim2.new(0, 10, 0, 10)
    wallpaperSliderKnob.Position = UDim2.new(winState.wallpaperOpacity, -5, 0.5, -5)
    wallpaperSliderKnob.ZIndex = 204
    wallpaperSliderKnob.Parent = wallpaperSliderTrack
    addCorner(wallpaperSliderKnob, 5)
    local wallpaperSliderHitBtn = Instance.new("TextButton")
    wallpaperSliderHitBtn.BackgroundTransparency = 1
    wallpaperSliderHitBtn.Size = UDim2.new(1, -12, 0, 18)
    wallpaperSliderHitBtn.Position = UDim2.new(0, 6, 0, 71)
    wallpaperSliderHitBtn.Text = ""
    wallpaperSliderHitBtn.ZIndex = 205
    wallpaperSliderHitBtn.AutoButtonColor = false
    wallpaperSliderHitBtn.Parent = wallpaperCardFrame
    local syncWallpaperOpacity = function()
        wallpaperOpacityBox.Text = tostring(math.floor(winState.wallpaperOpacity * 100)) .. "%"
        if wallpaperImage then
            wallpaperImage.ImageTransparency = 1 - winState.wallpaperOpacity
        end
    end
    local isDraggingWallpaper = false
    wallpaperOpacityBox.FocusLost:Connect(function()
        local c0 = tonumber(wallpaperOpacityBox.Text:match("%d+"))
        if c0 then
            local c1 = math.clamp(c0, 0, 100) / 100
            winState.wallpaperOpacity = c1
            wallpaperSliderFill.Size = UDim2.new(c1, 0, 1, 0)
            wallpaperSliderKnob.Position = UDim2.new(c1, -5, 0.5, -5)
            syncWallpaperOpacity()
            saveUISettings()
        else
            syncWallpaperOpacity()
        end
    end)
    wallpaperSliderHitBtn.InputBegan:Connect(function(c0)
        if (c0.UserInputType == Enum.UserInputType.MouseButton1) or (c0.UserInputType == Enum.UserInputType.Touch) then
            isDraggingWallpaper = true
            local c1 = math.clamp((c0.Position.X - wallpaperSliderTrack.AbsolutePosition.X) / wallpaperSliderTrack.AbsoluteSize.X, 0, 1)
            winState.wallpaperOpacity = c1
            wallpaperSliderFill.Size = UDim2.new(c1, 0, 1, 0)
            wallpaperSliderKnob.Position = UDim2.new(c1, -5, 0.5, -5)
            syncWallpaperOpacity()
            saveUISettings()
        end
    end)
    table.insert(winState.connections, UserInputService.InputChanged:Connect(function(c0)
        if isDraggingWallpaper and ((c0.UserInputType == Enum.UserInputType.MouseMovement) or (c0.UserInputType == Enum.UserInputType.Touch)) then
            local c1 = math.clamp((c0.Position.X - wallpaperSliderTrack.AbsolutePosition.X) / wallpaperSliderTrack.AbsoluteSize.X, 0, 1)
            winState.wallpaperOpacity = c1
            wallpaperSliderFill.Size = UDim2.new(c1, 0, 1, 0)
            wallpaperSliderKnob.Position = UDim2.new(c1, -5, 0.5, -5)
            syncWallpaperOpacity()
        end
    end))
    table.insert(winState.connections, UserInputService.InputEnded:Connect(function(c0)
        if (c0.UserInputType == Enum.UserInputType.MouseButton1) or (c0.UserInputType == Enum.UserInputType.Touch) then
            if isDraggingWallpaper then
                isDraggingWallpaper = false
                saveUISettings()
            end
        end
    end))
    local applyBgImageBtn = Instance.new("TextButton")
    applyBgImageBtn.BackgroundColor3 = palette.Accent
    applyBgImageBtn.Size = UDim2.new(1, -12, 0, 20)
    applyBgImageBtn.Position = UDim2.new(0, 6, 1, -52)
    local removeBgImageBtn = Instance.new("TextButton")
    removeBgImageBtn.BackgroundColor3 = Color3.fromRGB(90, 90, 90)
    removeBgImageBtn.Size = UDim2.new(1, -12, 0, 20)
    removeBgImageBtn.Position = UDim2.new(0, 6, 1, -28)
    removeBgImageBtn.FontFace = FontBold
    removeBgImageBtn.TextSize = 10
    removeBgImageBtn.TextColor3 = Color3.new(1, 1, 1)
    removeBgImageBtn.Text = "Remove Background Image"
    removeBgImageBtn.AutoButtonColor = false
    removeBgImageBtn.ZIndex = 202
    removeBgImageBtn.Parent = wallpaperCardFrame
    addCorner(removeBgImageBtn, 5)
    applyBgImageBtn.FontFace = FontBold
    applyBgImageBtn.TextSize = 10
    applyBgImageBtn.TextColor3 = Color3.new(1, 1, 1)
    applyBgImageBtn.Text = "Set Image In Background"
    applyBgImageBtn.AutoButtonColor = false
    applyBgImageBtn.ZIndex = 202
    applyBgImageBtn.Parent = wallpaperCardFrame
    addCorner(applyBgImageBtn, 5)
    onThemeChange(function()
        applyBgImageBtn.BackgroundColor3 = palette.Accent
    end)
    local runWallpaperTransition = function(c0)
        if closeConfigDrawer then
            closeConfigDrawer()
        end
        cancelGroupTweens("bg_change_anim")
        local c1 = TweenInfo.new(0.22, Enum.EasingStyle.Quart, Enum.EasingDirection.In)
        playGroupTween("bg_change_anim", mainFrame, c1, {
            BackgroundTransparency = 1,
        })
        playGroupTween("bg_change_anim", mainStroke, c1, {
            Transparency = 1,
        })
        local c2 = mainFrame:FindFirstChild("Shadow")
        if c2 then
            playGroupTween("bg_change_anim", c2, c1, {
                ImageTransparency = 1,
            })
        end
        task.delay(0.26, function()
            mainFrame.Visible = false
            if c0 then
                c0()
            end
            playLoadingScreen(palette, function()
                mainFrame.Visible = true
                cancelGroupTweens("bg_change_anim")
                playGroupTween("bg_change_anim", mainFrame, TweenInfo045, {
                    BackgroundTransparency = (winState.acrylicEnabled and winState.acrylicOpacity) or 0,
                })
                playGroupTween("bg_change_anim", mainStroke, TweenInfo045, {
                    Transparency = 0.6,
                })
                local e0 = mainFrame:FindFirstChild("Shadow")
                if e0 then
                    playGroupTween("bg_change_anim", e0, TweenInfo060, {
                        ImageTransparency = 0.5,
                    })
                end
            end)
        end)
    end
    applyBgImageBtn.MouseButton1Click:Connect(function()
        local c0 = tostring(bgImageInputBox.Text or ""):gsub("%s+", "")
        if c0 ~= "" then
            local c1 = c0:match("%d+")
            if c1 then
                runWallpaperTransition(function()
                    if wallpaperImage then
                        wallpaperImage.Image = "rbxassetid://" .. c1
                        wallpaperImage.Visible = true
                    end
                    winState.backgroundImageId = c1
                    uiSettings.backgroundImageId = c1
                    saveUISettings()
                end)
            end
        end
    end)
    removeBgImageBtn.MouseButton1Click:Connect(function()
        runWallpaperTransition(function()
            if wallpaperImage then
                wallpaperImage.Image = ""
                wallpaperImage.Visible = false
            end
            bgImageInputBox.Text = ""
            winState.backgroundImageId = ""
            uiSettings.backgroundImageId = ""
            saveUISettings()
        end)
    end)
    local overlayDividerLine = Instance.new("Frame")
    overlayDividerLine.BackgroundColor3 = palette.Border
    overlayDividerLine.BackgroundTransparency = 0.6
    overlayDividerLine.Size = UDim2.new(1, 0, 0, 1)
    overlayDividerLine.LayoutOrder = 8
    overlayDividerLine.BorderSizePixel = 0
    overlayDividerLine.ZIndex = 201
    overlayDividerLine.Parent = configDrawer
    bindThemeProp(overlayDividerLine, "BackgroundColor3", "Border")
    local overlaySectionTitle = Instance.new("TextLabel")
    overlaySectionTitle.BackgroundTransparency = 1
    overlaySectionTitle.Size = UDim2.new(1, 0, 0, 16)
    overlaySectionTitle.FontFace = FontMedium
    overlaySectionTitle.TextSize = 11
    overlaySectionTitle.TextColor3 = palette.TextWhite
    overlaySectionTitle.TextXAlignment = Enum.TextXAlignment.Left
    overlaySectionTitle.Text = "Overlay"
    overlaySectionTitle.LayoutOrder = 9
    overlaySectionTitle.ZIndex = 201
    overlaySectionTitle.Parent = configDrawer
    bindThemeProp(overlaySectionTitle, "TextColor3", "TextWhite")
    local settingsToggleSetters = {}
    local createSettingsToggle = function(c0, c1, c2, c3)
        local c4 = Instance.new("Frame")
        c4.BackgroundColor3 = palette.Background
        c4.BackgroundTransparency = 0.85
        c4.Size = UDim2.new(1, 0, 0, 34)
        c4.LayoutOrder = c1
        c4.ZIndex = 201
        c4.Parent = configDrawer
        addCorner(c4, 6)
        bindThemeProp(c4, "BackgroundColor3", "Background")
        local c5 = Instance.new("TextLabel")
        c5.BackgroundTransparency = 1
        c5.Size = UDim2.new(1, -60, 0, 18)
        c5.Position = UDim2.new(0, 6, 0.5, -9)
        c5.FontFace = FontBold
        c5.TextSize = 11
        c5.TextColor3 = palette.TextWhite
        c5.TextTransparency = 0.15
        c5.TextXAlignment = Enum.TextXAlignment.Left
        c5.Text = c0
        c5.ZIndex = 202
        c5.Parent = c4
        bindThemeProp(c5, "TextColor3", "TextWhite")
        local c6 = Instance.new("TextButton")
        c6.Size = UDim2.new(0, 44, 0, 22)
        c6.Position = UDim2.new(1, -50, 0.5, -11)
        c6.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
        c6.BackgroundTransparency = 0.2
        c6.Text = ""
        c6.AutoButtonColor = false
        c6.ZIndex = 202
        c6.Parent = c4
        addCorner(c6, 11)
        local c7 = Instance.new("Frame")
        c7.BackgroundColor3 = Color3.fromRGB(235, 235, 235)
        c7.BackgroundTransparency = 0.2
        c7.Size = UDim2.new(0, 16, 0, 16)
        c7.Position = UDim2.new(0, 3, 0.5, -8)
        c7.ZIndex = 203
        c7.Parent = c6
        addCorner(c7, 8)
        local c8 = false
        local c9 = function(d0)
            c8 = d0
            c6.BackgroundColor3 = (d0 and palette.Accent) or Color3.fromRGB(50, 50, 50)
            c7.Position = (d0 and UDim2.new(1, -19, 0.5, -8)) or UDim2.new(0, 3, 0.5, -8)
        end
        settingsToggleSetters[c0] = c9
        local c10 = "cfghov_" .. c0
        c4.InputBegan:Connect(function(d0)
            if d0.UserInputType == Enum.UserInputType.MouseMovement then
                cancelGroupTweens(c10)
                playGroupTween(c10, c5, TweenInfo020, {
                    TextTransparency = 0,
                })
                playGroupTween(c10, c6, TweenInfo020, {
                    BackgroundTransparency = 0,
                })
                playGroupTween(c10, c7, TweenInfo020, {
                    BackgroundTransparency = 0,
                })
                playGroupTween(c10, c4, TweenInfo020, {
                    BackgroundTransparency = 0.5,
                })
            end
        end)
        c4.InputEnded:Connect(function(d0)
            if d0.UserInputType == Enum.UserInputType.MouseMovement then
                cancelGroupTweens(c10)
                playGroupTween(c10, c5, TweenInfo020, {
                    TextTransparency = 0.15,
                })
                playGroupTween(c10, c6, TweenInfo020, {
                    BackgroundTransparency = 0.2,
                })
                playGroupTween(c10, c7, TweenInfo020, {
                    BackgroundTransparency = 0.2,
                })
                playGroupTween(c10, c4, TweenInfo020, {
                    BackgroundTransparency = 0.85,
                })
            end
        end)
        c6.MouseButton1Click:Connect(function()
            playSound(SOUND_OPEN)
            c8 = not c8
            local d0 = "cfgtog_" .. c0
            cancelGroupTweens(d0)
            playGroupTween(d0, c6, TweenInfo035, {
                BackgroundColor3 = (c8 and palette.Accent) or Color3.fromRGB(50, 50, 50),
            })
            playGroupTween(d0, c7, TweenInfo035, {
                Position = (c8 and UDim2.new(1, -19, 0.5, -8)) or UDim2.new(0, 3, 0.5, -8),
            })
            c2(c8)
            saveUISettings()
        end)
        onThemeChange(function()
            if c8 then
                c6.BackgroundColor3 = palette.Accent
            end
        end)
        if c3 then
            c9(true)
            task.defer(function()
                c2(true)
            end)
        end
        return c4
    end
    createSettingsToggle("Show Fps", 10, function(c0)
        showFps = c0
        updateFooterVisibility()
        if not c0 then
            fpsLabel.Text = "FPS: -"
        end
    end, uiSettings.showFps)
    createSettingsToggle("Show Ping", 11, function(c0)
        showPing = c0
        updateFooterVisibility()
        if not c0 then
            pingLabel.Text = "PING: -"
        end
    end, uiSettings.showPing)
    local playerDividerLine = Instance.new("Frame")
    playerDividerLine.BackgroundColor3 = palette.Border
    playerDividerLine.BackgroundTransparency = 0.6
    playerDividerLine.Size = UDim2.new(1, 0, 0, 1)
    playerDividerLine.LayoutOrder = 12
    playerDividerLine.BorderSizePixel = 0
    playerDividerLine.ZIndex = 201
    playerDividerLine.Parent = configDrawer
    bindThemeProp(playerDividerLine, "BackgroundColor3", "Border")
    local playerSectionTitle = Instance.new("TextLabel")
    playerSectionTitle.BackgroundTransparency = 1
    playerSectionTitle.Size = UDim2.new(1, 0, 0, 16)
    playerSectionTitle.FontFace = FontMedium
    playerSectionTitle.TextSize = 11
    playerSectionTitle.TextColor3 = palette.TextWhite
    playerSectionTitle.TextXAlignment = Enum.TextXAlignment.Left
    playerSectionTitle.Text = "Player"
    playerSectionTitle.LayoutOrder = 13
    playerSectionTitle.ZIndex = 201
    playerSectionTitle.Parent = configDrawer
    bindThemeProp(playerSectionTitle, "TextColor3", "TextWhite")
    local profilePanelFrame = Instance.new("Frame")
    profilePanelFrame.BackgroundColor3 = palette.Background
    profilePanelFrame.BackgroundTransparency = 1
    profilePanelFrame.Size = UDim2.new(0, SIDEBAR_WIDTH, 0, 64)
    profilePanelFrame.AnchorPoint = Vector2.new(0, 1)
    profilePanelFrame.Position = UDim2.new(0, 0, 1, 0)
    bindThemeProp(profilePanelFrame, "BackgroundColor3", "Background")
    profilePanelFrame.ZIndex = 4
    profilePanelFrame.Visible = false
    profilePanelFrame.ClipsDescendants = true
    profilePanelFrame.Parent = mainFrame
    local profileTopBorder = Instance.new("Frame")
    profileTopBorder.BackgroundColor3 = palette.Border
    profileTopBorder.BackgroundTransparency = 0.4
    profileTopBorder.Size = UDim2.new(1, 0, 0, 1)
    profileTopBorder.BorderSizePixel = 0
    profileTopBorder.ZIndex = 5
    profileTopBorder.Parent = profilePanelFrame
    bindThemeProp(profileTopBorder, "BackgroundColor3", "Border")
    local avatarImage = Instance.new("ImageLabel")
    avatarImage.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
    avatarImage.Size = UDim2.new(0, 38, 0, 38)
    avatarImage.Position = UDim2.new(0, 12, 0.5, -19)
    avatarImage.ZIndex = 5
    avatarImage.Parent = profilePanelFrame
    addCorner(avatarImage, 19)
    bindThemeProp(addStroke(avatarImage, palette.Border, 1.5, 0.3), "Color", "Border")
    local displayNameLabel = Instance.new("TextLabel")
    displayNameLabel.BackgroundTransparency = 1
    displayNameLabel.Size = UDim2.new(1, -62, 0, 15)
    displayNameLabel.Position = UDim2.new(0, 58, 0.5, -17)
    displayNameLabel.FontFace = FontBold
    displayNameLabel.TextSize = 12
    displayNameLabel.TextColor3 = palette.TextWhite
    displayNameLabel.TextXAlignment = Enum.TextXAlignment.Left
    displayNameLabel.TextTruncate = Enum.TextTruncate.AtEnd
    displayNameLabel.Text = LocalPlayer.DisplayName
    displayNameLabel.ZIndex = 5
    displayNameLabel.Parent = profilePanelFrame
    bindThemeProp(displayNameLabel, "TextColor3", "TextWhite")
    local usernameLabel = Instance.new("TextLabel")
    usernameLabel.BackgroundTransparency = 1
    usernameLabel.Size = UDim2.new(1, -62, 0, 12)
    usernameLabel.Position = UDim2.new(0, 58, 0.5, 1)
    usernameLabel.FontFace = FontMedium
    usernameLabel.TextSize = 10
    usernameLabel.TextColor3 = palette.AccentBright
    usernameLabel.TextTransparency = 0.1
    usernameLabel.TextXAlignment = Enum.TextXAlignment.Left
    usernameLabel.TextTruncate = Enum.TextTruncate.AtEnd
    usernameLabel.Text = "@" .. LocalPlayer.Name
    usernameLabel.ZIndex = 5
    usernameLabel.Parent = profilePanelFrame
    onThemeChange(function()
        usernameLabel.TextColor3 = palette.AccentBright
    end)
    task.spawn(function()
        local c0, c1 = pcall(function()
            return Players:GetUserThumbnailAsync(LocalPlayer.UserId, Enum.ThumbnailType.HeadShot, Enum.ThumbnailSize.Size60x60)
        end)
        if c0 and c1 then
            avatarImage.Image = c1
        end
    end)
    local setProfileVisible = function(c0)
        showProfile = c0
        if c0 then
            profilePanelFrame.Visible = true
            tabListScroll.Size = UDim2.new(0, SIDEBAR_WIDTH, 1, ((-HEADER_HEIGHT - 1) - searchBarHeight) - 64)
        else
            profilePanelFrame.Visible = false
            tabListScroll.Size = UDim2.new(0, SIDEBAR_WIDTH, 1, (-HEADER_HEIGHT - 1) - searchBarHeight)
        end
    end
    createSettingsToggle("Profile", 14, function(c0)
        setProfileVisible(c0)
    end, uiSettings.showProfile)
    local configBackdropBtn = Instance.new("TextButton")
    configBackdropBtn.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
    configBackdropBtn.BackgroundTransparency = 1
    configBackdropBtn.Size = UDim2.new(1, 0, 1, 0)
    configBackdropBtn.Text = ""
    configBackdropBtn.ZIndex = 195
    configBackdropBtn.Visible = false
    configBackdropBtn.AutoButtonColor = false
    configBackdropBtn.Parent = screenGui
    local dragStartInputPos = nil
    local dragStartFramePos = nil
    local resizeStartMousePos = nil
    local resizeStartWindowSize = nil
    local clampWindowPosition = function(c0)
        local c1 = c0.AbsoluteSize
        local c2 = screenGui.AbsoluteSize
        local c3 = c0.Position
        c0.Position = UDim2.new(0, math.clamp(c3.X.Offset + (c3.X.Scale * c2.X), -c1.X + 60, c2.X - 60), 0, math.clamp(c3.Y.Offset + (c3.Y.Scale * c2.Y), 0, c2.Y - HEADER_HEIGHT))
    end
    local headerDragButton = Instance.new("TextButton")
    headerDragButton.BackgroundTransparency = 1
    headerDragButton.Size = UDim2.new(0.55, 0, 1, 0)
    headerDragButton.Text = ""
    headerDragButton.ZIndex = 6
    headerDragButton.AutoButtonColor = false
    headerDragButton.Parent = contentHolder
    table.insert(winState.connections, headerDragButton.InputBegan:Connect(function(c0)
        if (c0.UserInputType == Enum.UserInputType.MouseButton1) or (c0.UserInputType == Enum.UserInputType.Touch) then
            winState.dragging = true
            dragStartInputPos = Vector2.new(c0.Position.X, c0.Position.Y)
            dragStartFramePos = mainFrame.Position
        end
    end))
    table.insert(winState.connections, UserInputService.InputChanged:Connect(function(c0)
        if winState.dragging and ((c0.UserInputType == Enum.UserInputType.MouseMovement) or (c0.UserInputType == Enum.UserInputType.Touch)) then
            local c1 = Vector2.new(c0.Position.X, c0.Position.Y) - dragStartInputPos
            local c2 = screenGui.AbsoluteSize
            mainFrame.Position = UDim2.new(0, (dragStartFramePos.X.Offset + (dragStartFramePos.X.Scale * c2.X)) + c1.X, 0, (dragStartFramePos.Y.Offset + (dragStartFramePos.Y.Scale * c2.Y)) + c1.Y)
        end
        if winState.resizing and ((c0.UserInputType == Enum.UserInputType.MouseMovement) or (c0.UserInputType == Enum.UserInputType.Touch)) then
            local c1 = Vector2.new(c0.Position.X, c0.Position.Y) - resizeStartMousePos
            mainFrame.Size = UDim2.new(0, math.clamp(resizeStartWindowSize.X + c1.X, MinWindowSize.X, MaxWindowSize.X), 0, math.clamp(resizeStartWindowSize.Y + c1.Y, MinWindowSize.Y, MaxWindowSize.Y))
        end
    end))
    table.insert(winState.connections, UserInputService.InputEnded:Connect(function(c0)
        if (c0.UserInputType == Enum.UserInputType.MouseButton1) or (c0.UserInputType == Enum.UserInputType.Touch) then
            if winState.dragging then
                winState.dragging = false
                clampWindowPosition(mainFrame)
            end
            if winState.resizing then
                winState.resizing = false
            end
        end
    end))
    table.insert(winState.connections, resizeHandle.InputBegan:Connect(function(c0)
        if (c0.UserInputType == Enum.UserInputType.MouseButton1) or (c0.UserInputType == Enum.UserInputType.Touch) then
            winState.resizing = true
            resizeStartMousePos = Vector2.new(c0.Position.X, c0.Position.Y)
            resizeStartWindowSize = mainFrame.AbsoluteSize
        end
    end))
    local isMinimizingAnim = false
    local savedChildVisibility = {}
    local restoreMinimizedWindow = function()
        for c3, c4 in ipairs(savedChildVisibility) do
            if c4.frame and c4.frame.Parent then
                c4.frame.LayoutOrder = c4.order
                c4.frame.Parent = c4.parent
            end
        end
        savedChildVisibility = {}
    end
    local switchTab = function(c0)
        if winState.selectedTab == c0 then
            return
        end
        winState.selectedTab = c0
        if searchTextBox and (searchTextBox.Text ~= "") then
            searchTextBox.Text = ""
        end
        if isMinimizingAnim then
            restoreMinimizedWindow()
            isMinimizingAnim = false
            searchResultsScroll.Visible = false
            pagesContainer.Visible = true
        end
        for c4, c5 in pairs(winState.tabs) do
            local c6 = c4 == c0
            local c7 = "tab_select_" .. c4
            cancelGroupTweens(c7)
            if c6 then
                playGroupTween(c7, c5.frame, TweenInfo035, {
                    BackgroundColor3 = palette.TabSelected,
                    BackgroundTransparency = 0.5,
                })
                playGroupTween(c7, c5.indicator, TweenInfo035, {
                    BackgroundTransparency = 0,
                    Size = UDim2.new(0, 3, 0.6, 0),
                })
                playGroupTween(c7, c5.titleLabel, TweenInfo035, {
                    TextColor3 = palette.AccentBright,
                    TextTransparency = 0,
                })
                playGroupTween(c7, c5.subtitleLabel, TweenInfo035, {
                    TextColor3 = palette.Accent,
                    TextTransparency = 0.1,
                })
                playGroupTween(c7, c5.iconLabel, TweenInfo035, {
                    ImageColor3 = palette.AccentBright,
                    ImageTransparency = 0,
                })
            else
                playGroupTween(c7, c5.frame, TweenInfo035, {
                    BackgroundColor3 = palette.TabDefault,
                    BackgroundTransparency = 1,
                })
                playGroupTween(c7, c5.indicator, TweenInfo035, {
                    BackgroundTransparency = 1,
                    Size = UDim2.new(0, 3, 0, 0),
                })
                playGroupTween(c7, c5.titleLabel, TweenInfo035, {
                    TextColor3 = palette.TextSubtitle,
                    TextTransparency = 0.45,
                })
                playGroupTween(c7, c5.subtitleLabel, TweenInfo035, {
                    TextColor3 = palette.TextSubtitle,
                    TextTransparency = 0.65,
                })
                playGroupTween(c7, c5.iconLabel, TweenInfo035, {
                    ImageColor3 = palette.TextSubtitle,
                    ImageTransparency = 0.6,
                })
            end
            if c5.page then
                c5.page.Visible = c6
            end
        end
    end
    local performSearch = function(c0)
        restoreMinimizedWindow()
        for c4, c5 in ipairs(searchResultsScroll:GetChildren()) do
            if (not c5:IsA("UIListLayout")) and (not c5:IsA("UIPadding")) then
                c5:Destroy()
            end
        end
        if c0 == "" then
            isMinimizingAnim = false
            searchResultsScroll.Visible = false
            pagesContainer.Visible = true
            return
        end
        isMinimizingAnim = true
        searchResultsScroll.Visible = true
        pagesContainer.Visible = false
        local c1 = c0:lower()
        local c2 = 0
        for c6, c7 in ipairs(winState.searchRegistry) do
            if c7.title:lower():find(c1, 1, true) or ((c7.desc ~= "") and c7.desc:lower():find(c1, 1, true)) then
                c2 = c2 + 1
                local c10 = c7.frame
                if c10 and c10.Parent then
                    table.insert(savedChildVisibility, {
                        frame = c10,
                        parent = c10.Parent,
                        order = c10.LayoutOrder,
                    })
                    c10.LayoutOrder = c2
                    c10.Parent = searchResultsScroll
                end
            end
        end
        if c2 == 0 then
            local c3 = Instance.new("TextLabel")
            c3.BackgroundTransparency = 1
            c3.Size = UDim2.new(1, 0, 0, 40)
            c3.LayoutOrder = 1
            c3.ZIndex = 11
            c3.FontFace = FontMedium
            c3.TextSize = 12
            c3.TextColor3 = palette.TextSubtitle
            c3.TextXAlignment = Enum.TextXAlignment.Center
            c3.Text = "No results found"
            c3.Parent = searchResultsScroll
        end
    end
    searchTextBox:GetPropertyChangedSignal("Text"):Connect(function()
        performSearch(searchTextBox.Text)
    end)
    searchTextBox.FocusLost:Connect(function()
        if searchTextBox.Text == "" then
            performSearch("")
        end
    end)
    local showNotification = nil
    local color3ToHex = nil
    local notificationsReady = false
    local queuedNotifications = {}
    local notifyWidth = 290
    local notifyRightMargin = 18
    local notifyBottomMargin = 18
    local notifySpacing = 8
    local notifyScreenGui = Instance.new("ScreenGui")
    notifyScreenGui.Name = "VexzHubNotify"
    notifyScreenGui.ResetOnSpawn = false
    notifyScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
    notifyScreenGui.IgnoreGuiInset = true
    notifyScreenGui.AutoLocalize = false
    notifyScreenGui.DisplayOrder = 30
    notifyScreenGui.Parent = PlayerGui
    local activeNotifications = {}
    local notifyIdCounter = 0
    color3ToHex = function(c0)
        return string.format("#%02X%02X%02X", math.floor((c0.R * 255) + 0.5), math.floor((c0.G * 255) + 0.5), math.floor((c0.B * 255) + 0.5))
    end
    showNotification = function(c0)
        c0 = c0 or {}
        if not notificationsReady then
            table.insert(queuedNotifications, c0)
            return
        end
        playSound(SOUND_TOGGLE)
        local c1 = c0.Title or "Notification"
        local c2 = c0.Text or ""
        local c3 = Lucide.Resolve(c0.Icon, "rbxassetid://124914698428562")
        local c4 = math.max(c0.Duration or 4, 0.5)
        local c5 = c0.RichText == true
        local c6 = c2 ~= ""
        local c7 = (c6 and 80) or 56
        notifyIdCounter = notifyIdCounter + 1
        local c8 = notifyIdCounter
        for c12, c13 in ipairs(activeNotifications) do
            c13.targetY = c13.targetY - (c7 + notifySpacing)
            cancelGroupTweens(c13.posKey)
            playGroupTween(c13.posKey, c13.frame, TweenInfo035, {
                Position = UDim2.new(1, -(notifyWidth + notifyRightMargin), 1, c13.targetY),
            })
        end
        local c9 = -notifyBottomMargin
        local c10 = Instance.new("Frame")
        c10.BackgroundColor3 = palette.Background
        c10.BackgroundTransparency = 0
        c10.Size = UDim2.new(0, notifyWidth, 0, c7)
        c10.AnchorPoint = Vector2.new(0, 1)
        c10.Position = UDim2.new(1, notifyRightMargin + notifyWidth, 1, c9)
        c10.ZIndex = 100
        c10.ClipsDescendants = true
        c10.Parent = notifyScreenGui
        addCorner(c10, 10)
        local c11 = addStroke(c10, palette.Border, 1, 0.3)
        addShadow(c10).ImageTransparency = 0.6
        local c13 = 52
        local c14 = Instance.new("Frame")
        c14.BackgroundColor3 = palette.AccentDeep
        c14.BackgroundTransparency = 1
        c14.Size = UDim2.new(0, c13, 1, -3)
        c14.Position = UDim2.new(0, 0, 0, 0)
        c14.BorderSizePixel = 0
        c14.ZIndex = 100
        c14.Parent = c10
        onThemeChange(function()
            if (not c14) or (not c14.Parent) then
                return
            end
            c14.BackgroundColor3 = palette.AccentDeep
        end)
        local c15 = 28
        local c16 = Instance.new("ImageLabel")
        c16.BackgroundTransparency = 1
        c16.Size = UDim2.new(0, c15, 0, c15)
        c16.AnchorPoint = Vector2.new(0.5, 0.5)
        c16.Position = UDim2.new(0, c13 / 2, 0.5, 0)
        c16.ScaleType = Enum.ScaleType.Fit
        local c17 = c0.IconColor
        c16.Image = c3
        c16.ImageColor3 = c17 or palette.Accent
        c16.ZIndex = 101
        c16.Parent = c10
        local c18 = Instance.new("Frame")
        c18.BackgroundColor3 = palette.Border
        c18.BackgroundTransparency = 0.25
        c18.BorderSizePixel = 0
        c18.Size = UDim2.new(0, 1, 1, -12)
        c18.Position = UDim2.new(0, c13, 0, 6)
        c18.ZIndex = 101
        c18.Parent = c10
        onThemeChange(function()
            if (not c18) or (not c18.Parent) then
                return
            end
            c18.BackgroundColor3 = palette.Border
        end)
        local c19 = (c6 and 10) or math.floor((c7 - 16) / 2)
        local c20 = Instance.new("TextLabel")
        c20.BackgroundTransparency = 1
        c20.Size = UDim2.new(1, -(c13 + 50), 0, 16)
        c20.Position = UDim2.new(0, c13 + 8, 0, c19)
        c20.FontFace = FontBold
        c20.TextSize = 12
        c20.TextColor3 = palette.AccentBright
        c20.TextXAlignment = Enum.TextXAlignment.Left
        c20.TextTruncate = Enum.TextTruncate.AtEnd
        c20.RichText = false
        c20.Text = c1
        c20.ZIndex = 101
        c20.Parent = c10
        local c21 = nil
        if c6 then
            c21 = Instance.new("TextLabel")
            c21.BackgroundTransparency = 1
            c21.Size = UDim2.new(1, -(c13 + 16), 0, 30)
            c21.Position = UDim2.new(0, c13 + 8, 0, 28)
            c21.FontFace = FontMedium
            c21.TextSize = 11
            c21.TextColor3 = Theme.TextWhite
            c21.TextTransparency = 0.1
            c21.TextXAlignment = Enum.TextXAlignment.Left
            c21.TextWrapped = true
            c21.RichText = c5
            c21.Text = c2
            c21.ZIndex = 101
            c21.Parent = c10
        end
        local c22 = Instance.new("Frame")
        c22.BackgroundColor3 = Color3.fromRGB(38, 38, 38)
        c22.BackgroundTransparency = 0.2
        c22.Size = UDim2.new(1, 0, 0, 3)
        c22.Position = UDim2.new(0, 0, 1, -3)
        c22.ZIndex = 101
        c22.Parent = c10
        addCorner(c22, 2)
        local c23 = Instance.new("Frame")
        c23.BackgroundColor3 = palette.Accent
        c23.Size = UDim2.new(1, 0, 1, 0)
        c23.ZIndex = 102
        c23.Parent = c22
        addCorner(c23, 2)
        local c24 = {}
        c24.frame = c10
        c24.targetY = c9
        c24.posKey = "npos_" .. c8
        c24.height = c7
        c24.iconLbl = c16
        c24.titleLbl = c20
        c24.bar = c23
        c24.nStroke = c11
        table.insert(activeNotifications, 1, c24)
        onThemeChange(function()
            if (not c10) or (not c10.Parent) then
                return
            end
            c10.BackgroundColor3 = palette.Background
            if not c0.IconColor then
                c16.ImageColor3 = palette.Accent
            end
            c20.TextColor3 = palette.AccentBright
            c23.BackgroundColor3 = palette.Accent
            c11.Color = palette.Border
            if c5 and c21 then
                c21.Text = string.gsub(c2, "color=\"#[%x]+\"", "color=\"" .. color3ToHex(palette.Accent) .. "\"")
            end
        end)
        local c25 = false
        local c26 = function()
            if (c25 or (not c10)) or (not c10.Parent) then
                return
            end
            c25 = true
            local d0 = c24.targetY
            for d4, d5 in ipairs(activeNotifications) do
                if d5.frame == c10 then
                    table.remove(activeNotifications, d4)
                    break
                end
            end
            for d4, d5 in ipairs(activeNotifications) do
                if d5.targetY < d0 then
                    d5.targetY = d5.targetY + (c7 + notifySpacing)
                    cancelGroupTweens(d5.posKey)
                    playGroupTween(d5.posKey, d5.frame, TweenInfo035, {
                        Position = UDim2.new(1, -(notifyWidth + notifyRightMargin), 1, d5.targetY),
                    })
                end
            end
            local d1 = c10.Position.Y.Offset
            cancelGroupTweens("nslide_" .. c8)
            local d2 = TweenInfo.new(0.22, Enum.EasingStyle.Quart, Enum.EasingDirection.In)
            TweenService:Create(c10, d2, {
                Position = UDim2.new(1, notifyRightMargin + notifyWidth, 1, d1),
                BackgroundTransparency = 1,
            }):Play()
            for d6, d7 in ipairs(c10:GetDescendants()) do
                if d7:IsA("TextLabel") then
                    TweenService:Create(d7, d2, {
                        TextTransparency = 1,
                    }):Play()
                elseif d7:IsA("ImageLabel") then
                    TweenService:Create(d7, d2, {
                        ImageTransparency = 1,
                    }):Play()
                elseif d7:IsA("Frame") then
                    TweenService:Create(d7, d2, {
                        BackgroundTransparency = 1,
                    }):Play()
                elseif d7:IsA("UIStroke") then
                    TweenService:Create(d7, d2, {
                        Transparency = 1,
                    }):Play()
                end
            end
            task.delay(0.26, function()
                if c10 and c10.Parent then
                    c10:Destroy()
                end
            end)
        end
        local c27 = Instance.new("TextButton")
        c27.BackgroundTransparency = 1
        c27.Size = UDim2.new(0, 18, 0, 18)
        c27.Position = UDim2.new(1, -24, 0, 6)
        c27.Text = "×"
        c27.TextSize = 16
        c27.FontFace = FontBold
        c27.TextColor3 = palette.TextWhite
        c27.TextTransparency = 0.3
        c27.ZIndex = 103
        c27.Parent = c10
        c27.MouseEnter:Connect(function()
            c27.TextTransparency = 0
        end)
        c27.MouseLeave:Connect(function()
            c27.TextTransparency = 0.3
        end)
        c27.MouseButton1Click:Connect(c26)
        playGroupTween("nslide_" .. c8, c10, TweenInfo035, {
            Position = UDim2.new(1, -(notifyWidth + notifyRightMargin), 1, c9),
        })
        TweenService:Create(c23, TweenInfo.new(c4, Enum.EasingStyle.Linear), {
            Size = UDim2.new(0, 0, 1, 0),
        }):Play()
        task.delay(c4, c26)
    end
    if type(self) == "table" then
        self._showNotification = showNotification
    end
    local showConfirmDialog = function(c0, c1, c2)
        modalOverlay.Visible = true
        modalOverlay.BackgroundTransparency = 1
        cancelGroupTweens(c1)
        playGroupTween(c1, modalOverlay, TweenInfo035, {
            BackgroundTransparency = 0.6,
        })
        local c3 = Instance.new("Frame")
        c3.BackgroundColor3 = palette.DialogBg
        c3.Size = UDim2.new(0, 280, 0, 130)
        c3.Position = UDim2.new(0.5, -140, 0.5, -65)
        c3.BackgroundTransparency = 1
        c3.ZIndex = 51
        c3.Parent = mainFrame
        addCorner(c3, 12)
        addStroke(c3, palette.Border, 1, 0.4)
        local c4 = addShadow(c3)
        c4.ImageTransparency = 1
        playGroupTween(c1, c3, TweenInfo035, {
            BackgroundTransparency = 0,
        })
        playGroupTween(c1, c4, TweenInfo035, {
            ImageTransparency = 0.5,
        })
        local c5 = Instance.new("TextLabel")
        c5.BackgroundTransparency = 1
        c5.Size = UDim2.new(1, -20, 0, 50)
        c5.Position = UDim2.new(0, 10, 0, 15)
        c5.FontFace = FontMedium
        c5.TextSize = 14
        c5.TextColor3 = palette.TextWhite
        c5.Text = c0
        c5.TextWrapped = true
        c5.TextTransparency = 1
        c5.ZIndex = 52
        c5.Parent = c3
        playGroupTween(c1, c5, TweenInfo035, {
            TextTransparency = 0,
        })
        local c6 = Instance.new("Frame")
        c6.BackgroundTransparency = 1
        c6.Size = UDim2.new(1, -30, 0, 36)
        c6.Position = UDim2.new(0, 15, 1, -52)
        c6.ZIndex = 52
        c6.Parent = c3
        local c7 = Instance.new("UIListLayout")
        c7.FillDirection = Enum.FillDirection.Horizontal
        c7.HorizontalAlignment = Enum.HorizontalAlignment.Center
        c7.Padding = UDim.new(0, 12)
        c7.Parent = c6
        local c8 = function(d0, d1)
            local d2 = Instance.new("TextButton")
            d2.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
            d2.Size = UDim2.new(0, 100, 0, 34)
            d2.FontFace = FontMedium
            d2.TextSize = 13
            d2.TextColor3 = palette.TextWhite
            d2.Text = d0
            d2.AutoButtonColor = false
            d2.LayoutOrder = d1
            d2.ZIndex = 53
            d2.BackgroundTransparency = 1
            d2.TextTransparency = 1
            d2.Parent = c6
            addCorner(d2, 8)
            addStroke(d2, palette.Border, 1, 0.6)
            playGroupTween(c1, d2, TweenInfo035, {
                BackgroundTransparency = 0,
                TextTransparency = 0,
            })
            local d3 = c1 .. "btn_" .. d0
            d2.MouseEnter:Connect(function()
                cancelGroupTweens(d3)
                playGroupTween(d3, d2, TweenInfo020, {
                    BackgroundColor3 = Color3.fromRGB(35, 35, 35),
                    Size = UDim2.new(0, 106, 0, 36),
                    TextColor3 = palette.Accent,
                })
            end)
            d2.MouseLeave:Connect(function()
                cancelGroupTweens(d3)
                playGroupTween(d3, d2, TweenInfo020, {
                    BackgroundColor3 = Color3.fromRGB(25, 25, 25),
                    Size = UDim2.new(0, 100, 0, 34),
                    TextColor3 = palette.TextWhite,
                })
            end)
            return d2
        end
        local c9 = c8("Yes", 1)
        local c10 = c8("No", 2)
        local c11 = function(d0)
            cancelGroupTweens(c1)
            local d1 = TweenInfo.new(0.26, Enum.EasingStyle.Quart, Enum.EasingDirection.In)
            playGroupTween(c1, c3, d1, {
                BackgroundTransparency = 1,
            })
            playGroupTween(c1, c5, d1, {
                TextTransparency = 1,
            })
            playGroupTween(c1, c9, d1, {
                BackgroundTransparency = 1,
                TextTransparency = 1,
            })
            playGroupTween(c1, c10, d1, {
                BackgroundTransparency = 1,
                TextTransparency = 1,
            })
            playGroupTween(c1, modalOverlay, d1, {
                BackgroundTransparency = 1,
            })
            if c4 then
                playGroupTween(c1, c4, d1, {
                    ImageTransparency = 1,
                })
            end
            task.delay(0.3, function()
                modalOverlay.Visible = false
                if c3 and c3.Parent then
                    c3:Destroy()
                end
                if d0 then
                    d0()
                end
            end)
        end
        c9.MouseButton1Click:Connect(function()
            c11(function()
                c2()
            end)
        end)
        c10.MouseButton1Click:Connect(function()
            c11(nil)
        end)
    end
    local toggleMinimizeWindow = function()
        showConfirmDialog("Do you want to dismiss the window?", "dialog_close", function()
            winState.destroyed = true
            for d3, d4 in pairs(winState.tabs) do
                if d4.stopTitleSlide then
                    d4.stopTitleSlide()
                end
                if d4.stopSubSlide then
                    d4.stopSubSlide()
                end
            end
            local d0 = TweenInfo.new(0.28, Enum.EasingStyle.Quart, Enum.EasingDirection.In)
            local d1 = Instance.new("UIScale")
            d1.Scale = 1
            d1.Parent = mainFrame
            playGroupTween("window_close", d1, d0, {
                Scale = 0.93,
            })
            playGroupTween("window_close", mainFrame, d0, {
                BackgroundTransparency = 1,
            })
            playGroupTween("window_close", mainStroke, d0, {
                Transparency = 1,
            })
            task.delay(0.34, function()
                for e3, e4 in ipairs(winState.connections) do
                    if typeof(e4) == "RBXScriptConnection" then
                        e4:Disconnect()
                    end
                end
                screenGui:Destroy()
                notifyScreenGui:Destroy()
            end)
        end)
    end
    table.insert(winState.connections, headerButtons.Close.MouseButton1Click:Connect(function()
        if not winState.destroyed then
            toggleMinimizeWindow()
        end
    end))
    table.insert(winState.connections, headerButtons.Maximize.MouseButton1Click:Connect(function()
        if winState.destroyed then
            return
        end
        cancelGroupTweens("maximize")
        if winState.maximized then
            winState.maximized = false
            playGroupTween("maximize", mainFrame, TweenInfo035, {
                Size = winState.preMaxSize,
                Position = winState.preMaxPos,
            })
            resizeHandle.Visible = true
        else
            winState.preMaxSize = mainFrame.Size
            winState.preMaxPos = mainFrame.Position
            winState.maximized = true
            local c0 = screenGui.AbsoluteSize
            playGroupTween("maximize", mainFrame, TweenInfo035, {
                Size = UDim2.new(0, c0.X, 0, c0.Y),
                Position = UDim2.new(0, 0, 0, 0),
            })
            resizeHandle.Visible = false
        end
    end))
    table.insert(winState.connections, headerButtons.Minimize.MouseButton1Click:Connect(function()
        if winState.destroyed then
            return
        end
        cancelGroupTweens("minimize")
        if winState.minimized then
            winState.minimized = false
            pagesContainer.Visible = true
            tabListScroll.Visible = true
            sidebarDivider.Visible = true
            resizeHandle.Visible = true
            searchBoxContainer.Visible = true
            if showProfile then
                profilePanelFrame.Visible = true
            end
            playGroupTween("minimize", mainFrame, TweenInfo035, {
                Size = winState.preMinSize,
            })
        else
            winState.preMinSize = mainFrame.Size
            winState.minimized = true
            playGroupTween("minimize", mainFrame, TweenInfo035, {
                Size = UDim2.new(0, mainFrame.AbsoluteSize.X, 0, HEADER_HEIGHT),
            })
            task.delay(0.38, function()
                if winState.minimized then
                    pagesContainer.Visible = false
                    tabListScroll.Visible = false
                    sidebarDivider.Visible = false
                    resizeHandle.Visible = false
                    searchBoxContainer.Visible = false
                    profilePanelFrame.Visible = false
                end
            end)
        end
    end))
    local getWindowTargetPos = function()
        local c0 = screenGui.AbsoluteSize
        local c1 = mainFrame.Position
        return Vector2.new((c1.X.Scale * c0.X) + c1.X.Offset, (c1.Y.Scale * c0.Y) + c1.Y.Offset)
    end
    local toggleConfigDrawer = function()
        if winState.configOpen then
            return
        end
        winState.configOpen = true
        local c0 = getWindowTargetPos()
        local c1 = mainFrame.AbsoluteSize
        configDrawer.Size = UDim2.new(0, 220, 0, (winState.minimized and 250) or c1.Y)
        configDrawer.Position = UDim2.new(0, c0.X + c1.X, 0, c0.Y)
        configDrawer.BackgroundTransparency = 1
        configDrawer.Visible = true
        configBackdropBtn.Visible = true
        configBackdropBtn.BackgroundTransparency = 1
        cancelGroupTweens("config")
        playGroupTween("config", configDrawer, TweenInfo035, {
            Position = UDim2.new(0, (c0.X + c1.X) + 8, 0, c0.Y),
            BackgroundTransparency = 0,
        })
        playGroupTween("config", configBackdropBtn, TweenInfo035, {
            BackgroundTransparency = 0.6,
        })
    end
    closeConfigDrawer = function()
        if not winState.configOpen then
            return
        end
        winState.configOpen = false
        cancelGroupTweens("config")
        local c0 = getWindowTargetPos()
        local c1 = mainFrame.AbsoluteSize
        local c2 = TweenInfo.new(0.26, Enum.EasingStyle.Quart, Enum.EasingDirection.In)
        playGroupTween("config", configDrawer, c2, {
            Position = UDim2.new(0, c0.X + c1.X, 0, c0.Y),
            BackgroundTransparency = 1,
        })
        playGroupTween("config", configBackdropBtn, c2, {
            BackgroundTransparency = 1,
        })
        task.delay(0.3, function()
            if not winState.configOpen then
                configDrawer.Visible = false
                configBackdropBtn.Visible = false
            end
        end)
    end
    table.insert(winState.connections, headerButtons.Config.MouseButton1Click:Connect(function()
        if not winState.destroyed then
            toggleConfigDrawer()
        end
    end))
    table.insert(winState.connections, configBackdropBtn.MouseButton1Click:Connect(function()
        closeConfigDrawer()
    end))
    local isWindowHidden = false
    local toggleWindowHidden = function()
        if winState.destroyed then
            return
        end
        isWindowHidden = not isWindowHidden
        mainFrame.Visible = not isWindowHidden
    end
    table.insert(winState.connections, UserInputService.InputBegan:Connect(function(c0, c1)
        if c1 then
            return
        end
        if (c0.KeyCode == Enum.KeyCode.LeftAlt) or (c0.KeyCode == Enum.KeyCode.LeftControl) then
            toggleWindowHidden()
        end
    end))
    local floatScreenGui = Instance.new("ScreenGui")
    floatScreenGui.Name = "VexzHubFloat"
    floatScreenGui.ResetOnSpawn = false
    floatScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
    floatScreenGui.IgnoreGuiInset = true
    floatScreenGui.AutoLocalize = false
    floatScreenGui.DisplayOrder = 10
    floatScreenGui.Parent = PlayerGui
    local floatToggleBtn = Instance.new("TextButton")
    floatToggleBtn.BackgroundColor3 = Color3.fromRGB(18, 18, 18)
    floatToggleBtn.BackgroundTransparency = 0
    floatToggleBtn.Size = UDim2.new(0, 50, 0, 50)
    floatToggleBtn.AnchorPoint = Vector2.new(0, 0)
    floatToggleBtn.Position = UDim2.new(1, -70, 1, -70)
    floatToggleBtn.Text = ""
    floatToggleBtn.AutoButtonColor = false
    floatToggleBtn.ZIndex = 1
    floatToggleBtn.Parent = floatScreenGui
    addCorner(floatToggleBtn, 25)
    local floatBtnStroke = addStroke(floatToggleBtn, palette.Accent, 1.5, 0.3)
    onThemeChange(function()
        floatBtnStroke.Color = palette.Accent
    end)
    if windowIcon ~= "" then
        local b188 = Instance.new("ImageLabel")
        b188.BackgroundTransparency = 1
        b188.Size = UDim2.new(1, 0, 1, 0)
        b188.Image = windowIcon
        b188.ImageColor3 = Color3.new(1, 1, 1)
        b188.ScaleType = Enum.ScaleType.Crop
        b188.ZIndex = 2
        b188.Parent = floatToggleBtn
        addCorner(b188, 25)
    end
    local isDraggingFloatBtn = false
    local floatDragStartPos = Vector2.new(0, 0)
    local floatStartUDimPos = floatToggleBtn.Position
    local floatDragMoved = false
    local activeFloatInput = nil
    floatToggleBtn.InputBegan:Connect(function(c0)
        if (c0.UserInputType == Enum.UserInputType.Touch) or (c0.UserInputType == Enum.UserInputType.MouseButton1) then
            if activeFloatInput ~= nil then
                return
            end
            activeFloatInput = c0
            isDraggingFloatBtn = true
            floatDragMoved = false
            floatDragStartPos = Vector2.new(c0.Position.X, c0.Position.Y)
            floatStartUDimPos = floatToggleBtn.Position
        end
    end)
    table.insert(winState.connections, UserInputService.InputChanged:Connect(function(c0)
        if (not isDraggingFloatBtn) or (c0 ~= activeFloatInput) then
            return
        end
        local c1 = Vector2.new(c0.Position.X, c0.Position.Y) - floatDragStartPos
        if c1.Magnitude > 6 then
            floatDragMoved = true
        end
        local c2 = floatScreenGui.AbsoluteSize
        floatToggleBtn.Position = UDim2.new(0, math.clamp((floatStartUDimPos.X.Offset + (floatStartUDimPos.X.Scale * c2.X)) + c1.X, 0, c2.X - 50), 0, math.clamp((floatStartUDimPos.Y.Offset + (floatStartUDimPos.Y.Scale * c2.Y)) + c1.Y, 0, c2.Y - 50))
    end))
    table.insert(winState.connections, UserInputService.InputEnded:Connect(function(c0)
        if c0 ~= activeFloatInput then
            return
        end
        if isDraggingFloatBtn and (not floatDragMoved) then
            toggleWindowHidden()
        end
        isDraggingFloatBtn = false
        activeFloatInput = nil
    end))
    floatToggleBtn.MouseEnter:Connect(function()
        cancelGroupTweens("fb_hover")
        playGroupTween("fb_hover", floatToggleBtn, TweenInfo020, {
            BackgroundTransparency = 0.15,
        })
    end)
    floatToggleBtn.MouseLeave:Connect(function()
        cancelGroupTweens("fb_hover")
        playGroupTween("fb_hover", floatToggleBtn, TweenInfo020, {
            BackgroundTransparency = 0,
        })
    end)
    task.delay(0.1, function()
        playSound(SOUND_CLICK)
        mainFrame.Visible = true
        cancelGroupTweens("window_open")
        if uiSettings.acrylicEnabled then
            winState.acrylicEnabled = true
            winState.acrylicOpacity = uiSettings.acrylicOpacity
            acrylicToggleBtn.BackgroundColor3 = palette.Accent
            acrylicToggleKnob.Position = UDim2.new(1, -19, 0.5, -8)
            local c0 = uiSettings.acrylicOpacity
            opacitySliderFill.Size = UDim2.new(c0, 0, 1, 0)
            opacitySliderKnob.Position = UDim2.new(c0, -6, 0.5, -6)
            opacityInputBox.Text = tostring(math.floor(c0 * 100)) .. "%"
            playGroupTween("window_open", mainFrame, TweenInfo045, {
                Size = UDim2.new(0, windowSize.X, 0, windowSize.Y),
                BackgroundTransparency = c0,
            })
        else
            playGroupTween("window_open", mainFrame, TweenInfo045, {
                Size = UDim2.new(0, windowSize.X, 0, windowSize.Y),
                BackgroundTransparency = 0,
            })
        end
        if ((uiSettings.theme == "Custom") and uiSettings.customColorHex) and (uiSettings.customColorHex ~= "") then
            local c0 = uiSettings.customColorHex:gsub("#", "")
            local c1 = tonumber(c0:sub(1, 2), 16)
            local c2 = tonumber(c0:sub(3, 4), 16)
            local c3 = tonumber(c0:sub(5, 6), 16)
            if (c1 and c2) and c3 then
                winState.customColorHex = uiSettings.customColorHex
                local c4 = Color3.fromRGB(c1, c2, c3)
                applyThemePalette(c4)
                setColorPickerFromColor(c4)
            end
        elseif (uiSettings.theme ~= currentThemeName) and ColorPresets[uiSettings.theme] then
            applyThemePalette(uiSettings.theme)
        end
        winState.wallpaperOpacity = uiSettings.wallpaperOpacity
        wallpaperSliderFill.Size = UDim2.new(winState.wallpaperOpacity, 0, 1, 0)
        wallpaperSliderKnob.Position = UDim2.new(winState.wallpaperOpacity, -5, 0.5, -5)
        wallpaperOpacityBox.Text = tostring(math.floor(winState.wallpaperOpacity * 100)) .. "%"
        if uiSettings.backgroundImageId and (uiSettings.backgroundImageId ~= "") then
            winState.backgroundImageId = uiSettings.backgroundImageId
            bgImageInputBox.Text = uiSettings.backgroundImageId
            if wallpaperImage then
                wallpaperImage.Image = "rbxassetid://" .. uiSettings.backgroundImageId
                wallpaperImage.Visible = true
            end
        end
        if wallpaperImage then
            wallpaperImage.ImageTransparency = 1 - winState.wallpaperOpacity
        end
        playGroupTween("window_open", mainStroke, TweenInfo045, {
            Transparency = 0.6,
        })
        playGroupTween("window_open", mainShadow, TweenInfo060, {
            ImageTransparency = 0.5,
        })
        notificationsReady = true
        for c3, c4 in ipairs(deferredLoaders) do
            task.spawn(c4)
        end
        deferredLoaders = {}
        for c3, c4 in ipairs(queuedNotifications) do
            task.delay((c3 - 1) * 0.15, function()
                if showNotification then
                    showNotification(c4)
                end
            end)
        end
        queuedNotifications = {}
    end)
    local tabOrderCounter = 0
    return (function()
        local createTab = function(self, tabOpts, iconArg, subArg)
            local tabConfig
            if type(tabOpts) == "table" then
                tabConfig = tabOpts
            elseif subArg ~= nil then
                tabConfig = {
                    Title = tostring(tabOpts or "Tab"),
                    Subtitle = tostring(iconArg or ""),
                    Icon = subArg,
                }
            else
                tabConfig = {
                    Title = tostring(tabOpts or "Tab"),
                    Icon = iconArg,
                }
            end
            local tabTitle = tabConfig.Title or tabConfig.Name or "Tab"
            local tabSubtitle = tabConfig.Subtitle or tabConfig.SubTitle or tabConfig.Description or ""
            local rawTabIcon = tabConfig.Icon
            if rawTabIcon == nil then
                rawTabIcon = tabConfig.icon
            end
            if rawTabIcon == nil then
                rawTabIcon = iconArg
            end
            local tabIcon = Lucide.ResolveTabIcon(rawTabIcon, tabTitle, tabSubtitle)
            local hasTabIcon = tabIcon ~= ""
            tabOrderCounter = tabOrderCounter + 1
            local tabButton = Instance.new("TextButton")
            tabButton.BackgroundColor3 = palette.TabDefault
            tabButton.BackgroundTransparency = 1
            tabButton.Size = UDim2.new(1, -8, 0, ELEMENT_HEIGHT)
            tabButton.AutoButtonColor = false
            tabButton.Text = ""
            tabButton.LayoutOrder = tabOrderCounter
            tabButton.ZIndex = 4
            tabButton.Parent = tabListScroll
            addCorner(tabButton, 6)
            local tabIndicator = Instance.new("Frame")
            tabIndicator.BackgroundColor3 = palette.Accent
            tabIndicator.BackgroundTransparency = 1
            tabIndicator.Size = UDim2.new(0, 3, 0, 0)
            tabIndicator.Position = UDim2.new(0, 0, 0.2, 0)
            tabIndicator.BorderSizePixel = 0
            tabIndicator.ZIndex = 5
            tabIndicator.Parent = tabButton
            addCorner(tabIndicator, 2)
            onThemeChange(function()
                tabIndicator.BackgroundColor3 = palette.Accent
            end)
            local tabIconLabel = Instance.new("ImageLabel")
            tabIconLabel.BackgroundTransparency = 1
            tabIconLabel.Size = UDim2.new(0, ICON_SIZE_X, 0, ICON_SIZE_X)
            tabIconLabel.Position = UDim2.new(0, 10, 0.5, -ICON_SIZE_X / 2)
            tabIconLabel.ScaleType = Enum.ScaleType.Fit
            tabIconLabel.Image = tabIcon
            tabIconLabel.ImageColor3 = palette.TextSubtitle
            tabIconLabel.ImageTransparency = 0.6
            tabIconLabel.Visible = hasTabIcon
            tabIconLabel.ZIndex = 5
            tabIconLabel.Parent = tabButton
            local tabTextContainer = Instance.new("Frame")
            tabTextContainer.BackgroundTransparency = 1
            tabTextContainer.Size = (hasTabIcon and UDim2.new(1, -ICON_SIZE_X - 22, 0, ELEMENT_HEIGHT - 8)) or UDim2.new(1, -20, 0, ELEMENT_HEIGHT - 8)
            tabTextContainer.Position = (hasTabIcon and UDim2.new(0, ICON_SIZE_X + 16, 0.5, -(ELEMENT_HEIGHT - 8) / 2)) or UDim2.new(0, 12, 0.5, -(ELEMENT_HEIGHT - 8) / 2)
            tabTextContainer.ClipsDescendants = true
            tabTextContainer.ZIndex = 5
            tabTextContainer.Parent = tabButton
            local tabTextLayout = Instance.new("UIListLayout")
            tabTextLayout.FillDirection = Enum.FillDirection.Vertical
            tabTextLayout.VerticalAlignment = Enum.VerticalAlignment.Center
            tabTextLayout.Padding = UDim.new(0, 0)
            tabTextLayout.SortOrder = Enum.SortOrder.LayoutOrder
            tabTextLayout.Parent = tabTextContainer
            local tabTitleClip = Instance.new("Frame")
            tabTitleClip.BackgroundTransparency = 1
            tabTitleClip.Size = ((tabSubtitle ~= "") and UDim2.new(1, 0, 0, 13)) or UDim2.new(1, 0, 0, 15)
            tabTitleClip.ClipsDescendants = true
            tabTitleClip.LayoutOrder = 1
            tabTitleClip.ZIndex = 5
            tabTitleClip.Parent = tabTextContainer
            local tabTitleLabel = Instance.new("TextLabel")
            tabTitleLabel.BackgroundTransparency = 1
            tabTitleLabel.Size = UDim2.new(2, 0, 1, 0)
            tabTitleLabel.FontFace = FontBold
            tabTitleLabel.TextSize = 12
            tabTitleLabel.TextColor3 = palette.TextSubtitle
            tabTitleLabel.TextTransparency = 0.45
            tabTitleLabel.TextXAlignment = Enum.TextXAlignment.Left
            tabTitleLabel.AutomaticSize = Enum.AutomaticSize.X
            tabTitleLabel.Text = tabTitle
            tabTitleLabel.ZIndex = 6
            tabTitleLabel.Parent = tabTitleClip
            local tabSubtitleClip = Instance.new("Frame")
            tabSubtitleClip.BackgroundTransparency = 1
            tabSubtitleClip.Size = UDim2.new(1, 0, 0, 11)
            tabSubtitleClip.ClipsDescendants = true
            tabSubtitleClip.LayoutOrder = 2
            tabSubtitleClip.ZIndex = 5
            tabSubtitleClip.Visible = tabSubtitle ~= ""
            tabSubtitleClip.Parent = tabTextContainer
            local tabSubtitleLabel = Instance.new("TextLabel")
            tabSubtitleLabel.BackgroundTransparency = 1
            tabSubtitleLabel.Size = UDim2.new(2, 0, 1, 0)
            tabSubtitleLabel.FontFace = FontBold
            tabSubtitleLabel.TextSize = 9
            tabSubtitleLabel.TextColor3 = palette.TextSubtitle
            tabSubtitleLabel.TextTransparency = 0.65
            tabSubtitleLabel.TextXAlignment = Enum.TextXAlignment.Left
            tabSubtitleLabel.AutomaticSize = Enum.AutomaticSize.X
            tabSubtitleLabel.Text = tabSubtitle
            tabSubtitleLabel.ZIndex = 6
            tabSubtitleLabel.Parent = tabSubtitleClip
            local stopTitleMarquee = startMarqueeScroll(tabTitleLabel, tabTitleClip)
            local stopSubMarquee = startMarqueeScroll(tabSubtitleLabel, tabSubtitleClip)
            local tabPageScroll = Instance.new("ScrollingFrame")
            tabPageScroll.BackgroundTransparency = 1
            tabPageScroll.Size = UDim2.new(1, 0, 1, 0)
            tabPageScroll.Visible = false
            tabPageScroll.ZIndex = 2
            tabPageScroll.BorderSizePixel = 0
            tabPageScroll.ScrollBarThickness = 2
            tabPageScroll.ScrollBarImageColor3 = MutedTextColor
            tabPageScroll.ScrollBarImageTransparency = 0.5
            tabPageScroll.CanvasSize = UDim2.new(0, 0, 0, 0)
            tabPageScroll.AutomaticCanvasSize = Enum.AutomaticSize.Y
            tabPageScroll.Parent = pagesContainer
            local tabPageLayout = Instance.new("UIListLayout")
            tabPageLayout.FillDirection = Enum.FillDirection.Vertical
            tabPageLayout.Padding = UDim.new(0, 8)
            tabPageLayout.SortOrder = Enum.SortOrder.LayoutOrder
            tabPageLayout.Parent = tabPageScroll
            addPadding(tabPageScroll, 12, 14, 12, 12)
            winState.tabs[tabTitle] = {
                frame = tabButton,
                indicator = tabIndicator,
                titleLabel = tabTitleLabel,
                subtitleLabel = tabSubtitleLabel,
                iconLabel = tabIconLabel,
                page = tabPageScroll,
                stopTitleSlide = stopTitleMarquee,
                stopSubSlide = stopSubMarquee,
            }
            local tabTweenPrefix = "tab_" .. tabTitle
            tabButton.MouseEnter:Connect(function()
                if winState.selectedTab == tabTitle then
                    return
                end
                cancelGroupTweens(tabTweenPrefix .. "_h")
                playGroupTween(tabTweenPrefix .. "_h", tabButton, TweenInfo020, {
                    BackgroundColor3 = palette.TabHover,
                    BackgroundTransparency = 0.7,
                })
                playGroupTween(tabTweenPrefix .. "_h", tabTitleLabel, TweenInfo020, {
                    TextTransparency = 0.2,
                })
                playGroupTween(tabTweenPrefix .. "_h", tabIconLabel, TweenInfo020, {
                    ImageTransparency = 0.3,
                })
            end)
            tabButton.MouseLeave:Connect(function()
                if winState.selectedTab == tabTitle then
                    return
                end
                cancelGroupTweens(tabTweenPrefix .. "_h")
                playGroupTween(tabTweenPrefix .. "_h", tabButton, TweenInfo020, {
                    BackgroundColor3 = palette.TabDefault,
                    BackgroundTransparency = 1,
                })
                playGroupTween(tabTweenPrefix .. "_h", tabTitleLabel, TweenInfo020, {
                    TextTransparency = 0.45,
                })
                playGroupTween(tabTweenPrefix .. "_h", tabIconLabel, TweenInfo020, {
                    ImageTransparency = 0.6,
                })
            end)
            tabButton.MouseButton1Click:Connect(function()
                if not winState.destroyed then
                    playSound(SOUND_OPEN)
                    switchTab(tabTitle)
                end
            end)
            if not winState.selectedTab then
                switchTab(tabTitle)
            end
            local elementOrder = 0
            local registerSearchItem = function(d0, d1, d2)
                table.insert(winState.searchRegistry, {
                    title = d0,
                    desc = d1 or "",
                    description = d1 or "",
                    frame = d2,
                    tabName = tabTitle,
                })
            end
            return {
                SetIcon = function(self, newIcon)
                    local updatedIcon = Lucide.ResolveTabIcon(newIcon, tabTitle, tabSubtitle)
                    local showIcon = updatedIcon ~= ""
                    tabIconLabel.Image = updatedIcon
                    tabIconLabel.Visible = showIcon
                    tabTextContainer.Size = (showIcon and UDim2.new(1, -ICON_SIZE_X - 22, 0, ELEMENT_HEIGHT - 8)) or UDim2.new(1, -20, 0, ELEMENT_HEIGHT - 8)
                    tabTextContainer.Position = (showIcon and UDim2.new(0, ICON_SIZE_X + 16, 0.5, -(ELEMENT_HEIGHT - 8) / 2)) or UDim2.new(0, 12, 0.5, -(ELEMENT_HEIGHT - 8) / 2)
                end,
                AddSection = function(self, sectionTitle)
                    elementOrder = elementOrder + 1
                    local sectionHeaderFrame = Instance.new("Frame")
                    sectionHeaderFrame.BackgroundTransparency = 1
                    sectionHeaderFrame.Size = UDim2.new(1, 0, 0, 22)
                    sectionHeaderFrame.LayoutOrder = elementOrder
                    sectionHeaderFrame.ZIndex = 3
                    sectionHeaderFrame.Parent = tabPageScroll
                    local sectionAccentBar = Instance.new("Frame")
                    sectionAccentBar.BackgroundColor3 = palette.Accent
                    sectionAccentBar.BackgroundTransparency = 0.35
                    sectionAccentBar.Size = UDim2.new(0, 2, 0, 14)
                    sectionAccentBar.Position = UDim2.new(0, 2, 0.5, -7)
                    sectionAccentBar.BorderSizePixel = 0
                    sectionAccentBar.ZIndex = 4
                    sectionAccentBar.Parent = sectionHeaderFrame
                    addCorner(sectionAccentBar, 1)
                    onThemeChange(function()
                        sectionAccentBar.BackgroundColor3 = palette.Accent
                    end)
                    local sectionTitleLabel = Instance.new("TextLabel")
                    sectionTitleLabel.BackgroundTransparency = 1
                    sectionTitleLabel.Size = UDim2.new(1, -12, 1, 0)
                    sectionTitleLabel.Position = UDim2.new(0, 10, 0, 0)
                    sectionTitleLabel.FontFace = FontBold
                    sectionTitleLabel.TextSize = 11
                    sectionTitleLabel.TextColor3 = palette.TextWhite
                    sectionTitleLabel.TextTransparency = 0.35
                    sectionTitleLabel.TextXAlignment = Enum.TextXAlignment.Left
                    sectionTitleLabel.Text = sectionTitle or ""
                    sectionTitleLabel.ZIndex = 4
                    sectionTitleLabel.Parent = sectionHeaderFrame
                    bindThemeProp(sectionTitleLabel, "TextColor3", "TextWhite")
                    local sectionApi = {}
                    local wrapAutoSave = function(e0, e1)
                        if not e0 then
                            return e0
                        end
                        if _G and _G.AutoLoadHook then
                            local e2 = _G.AutoLoadHook(e1, nil)
                            if e2 ~= nil then
                                e0.Default = e2
                            end
                        end
                        local e2 = e0.Callback or function() end
                        e0.Callback = function(f0, ...)
                            if _G and _G.AutoSaveHook then
                                _G.AutoSaveHook(e1, f0)
                            end
                            return e2(f0, ...)
                        end
                        return e0
                    end
                    local makeComponentKey = function(e0)
                        return "NM_" .. tostring(e0 or ""):gsub("[^%w]", "_")
                    end
                    sectionApi.AddToggle = function(self, toggleOpts)
                        toggleOpts = toggleOpts or {}
                        local toggleTitle = toggleOpts.Title or "Toggle"
                        local toggleDesc = toggleOpts.Description or ""
                        local defaultState = ((toggleOpts.Default ~= nil) and toggleOpts.Default) or false
                        local callback = toggleOpts.Callback or function() end
                        local currentState = defaultState
                        elementOrder = elementOrder + 1
                        local toggleFrame = Instance.new("Frame")
                        toggleFrame.BackgroundColor3 = palette.Background
                        toggleFrame.BackgroundTransparency = 0.85
                        if toggleDesc ~= "" then
                            toggleFrame.Size = UDim2.new(1, 0, 0, 0)
                            toggleFrame.AutomaticSize = Enum.AutomaticSize.Y
                        else
                            toggleFrame.Size = UDim2.new(1, 0, 0, 34)
                        end
                        toggleFrame.LayoutOrder = elementOrder
                        toggleFrame.ZIndex = 3
                        toggleFrame.Parent = tabPageScroll
                        applyHoverGlow(toggleFrame, "tog_" .. toggleTitle .. elementOrder)
                        bindThemeProp(toggleFrame, "BackgroundColor3", "Background")
                        local titleLabel = Instance.new("TextLabel")
                        titleLabel.BackgroundTransparency = 1
                        titleLabel.Size = UDim2.new(1, -60, 0, 18)
                        if toggleDesc ~= "" then
                            titleLabel.Position = UDim2.new(0, 6, 0, 8)
                        else
                            titleLabel.AnchorPoint = Vector2.new(0, 0.5)
                            titleLabel.Position = UDim2.new(0, 6, 0.5, 0)
                        end
                        titleLabel.FontFace = FontBold
                        titleLabel.TextSize = 13
                        titleLabel.TextColor3 = palette.TextWhite
                        titleLabel.TextTransparency = 0.15
                        titleLabel.TextXAlignment = Enum.TextXAlignment.Left
                        titleLabel.Text = toggleTitle
                        titleLabel.ZIndex = 4
                        titleLabel.Parent = toggleFrame
                        bindThemeProp(titleLabel, "TextColor3", "TextWhite")
                        if toggleDesc ~= "" then
                            local e9 = Instance.new("TextLabel")
                            e9.BackgroundTransparency = 1
                            e9.Size = UDim2.new(1, -60, 0, 0)
                            e9.AutomaticSize = Enum.AutomaticSize.Y
                            e9.Position = UDim2.new(0, 6, 0, 28)
                            e9.FontFace = FontMedium
                            e9.TextSize = 11
                            e9.TextColor3 = palette.TextSubtitle
                            e9.TextXAlignment = Enum.TextXAlignment.Left
                            e9.TextWrapped = true
                            e9.Text = toggleDesc
                            e9.ZIndex = 4
                            e9.Parent = toggleFrame
                            bindThemeProp(e9, "TextColor3", "TextSubtitle")
                            local e10 = Instance.new("UIPadding")
                            e10.PaddingBottom = UDim.new(0, 8)
                            e10.Parent = toggleFrame
                        end
                        local switchTrackBtn = Instance.new("TextButton")
                        switchTrackBtn.BackgroundColor3 = (currentState and palette.Accent) or Color3.fromRGB(50, 50, 50)
                        switchTrackBtn.BackgroundTransparency = 0.2
                        switchTrackBtn.Size = UDim2.new(0, 44, 0, 22)
                        switchTrackBtn.Position = ((toggleDesc ~= "") and UDim2.new(1, -50, 0, 8)) or UDim2.new(1, -50, 0.5, -11)
                        switchTrackBtn.Text = ""
                        switchTrackBtn.AutoButtonColor = false
                        switchTrackBtn.ZIndex = 4
                        switchTrackBtn.Parent = toggleFrame
                        addCorner(switchTrackBtn, 11)
                        onThemeChange(function()
                            if currentState then
                                switchTrackBtn.BackgroundColor3 = palette.Accent
                            end
                        end)
                        local switchKnob = Instance.new("Frame")
                        switchKnob.BackgroundColor3 = palette.TextWhite
                        switchKnob.BackgroundTransparency = 0.2
                        switchKnob.Size = UDim2.new(0, 16, 0, 16)
                        switchKnob.Position = (currentState and UDim2.new(1, -19, 0.5, -8)) or UDim2.new(0, 3, 0.5, -8)
                        switchKnob.ZIndex = 5
                        switchKnob.Parent = switchTrackBtn
                        addCorner(switchKnob, 8)
                        local hoverGroupKey = "toghov_" .. toggleTitle .. elementOrder
                        toggleFrame.InputBegan:Connect(function(f0)
                            if f0.UserInputType == Enum.UserInputType.MouseMovement then
                                cancelGroupTweens(hoverGroupKey)
                                playGroupTween(hoverGroupKey, titleLabel, TweenInfo020, {
                                    TextTransparency = 0,
                                })
                                playGroupTween(hoverGroupKey, switchTrackBtn, TweenInfo020, {
                                    BackgroundTransparency = 0,
                                })
                                playGroupTween(hoverGroupKey, switchKnob, TweenInfo020, {
                                    BackgroundTransparency = 0,
                                })
                                playGroupTween(hoverGroupKey, toggleFrame, TweenInfo020, {
                                    BackgroundTransparency = 0.5,
                                })
                            end
                        end)
                        toggleFrame.InputEnded:Connect(function(f0)
                            if f0.UserInputType == Enum.UserInputType.MouseMovement then
                                cancelGroupTweens(hoverGroupKey)
                                playGroupTween(hoverGroupKey, titleLabel, TweenInfo020, {
                                    TextTransparency = 0.15,
                                })
                                playGroupTween(hoverGroupKey, switchTrackBtn, TweenInfo020, {
                                    BackgroundTransparency = 0.2,
                                })
                                playGroupTween(hoverGroupKey, switchKnob, TweenInfo020, {
                                    BackgroundTransparency = 0.2,
                                })
                                playGroupTween(hoverGroupKey, toggleFrame, TweenInfo020, {
                                    BackgroundTransparency = 0.85,
                                })
                            end
                        end)
                        local toggleValue = function()
                            local f0 = "toggle_" .. toggleTitle .. elementOrder
                            cancelGroupTweens(f0)
                            if currentState then
                                playGroupTween(f0, switchTrackBtn, TweenInfo035, {
                                    BackgroundColor3 = palette.Accent,
                                })
                                playGroupTween(f0, switchKnob, TweenInfo035, {
                                    Position = UDim2.new(1, -19, 0.5, -8),
                                })
                            else
                                playGroupTween(f0, switchTrackBtn, TweenInfo035, {
                                    BackgroundColor3 = Color3.fromRGB(50, 50, 50),
                                })
                                playGroupTween(f0, switchKnob, TweenInfo035, {
                                    Position = UDim2.new(0, 3, 0.5, -8),
                                })
                            end
                        end
                        switchTrackBtn.MouseButton1Click:Connect(function()
                            playSound(SOUND_OPEN)
                            currentState = not currentState
                            toggleValue()
                            callback(currentState)
                        end)
                        local toggleApi = {
                            Set = function(f0, f1)
                                currentState = f1
                                toggleValue()
                                callback(currentState)
                            end,
                            Get = function(f0)
                                return currentState
                            end,
                            SetTitle = function(f0, f1)
                                titleLabel.Text = f1
                            end,
                            GetFrame = function(f0)
                                return toggleFrame
                            end,
                        }
                        if defaultState then
                            task.defer(function()
                                callback(currentState)
                            end)
                        end
                        registerSearchItem(toggleTitle, toggleDesc, toggleFrame)
                        registerComponent(toggleOpts.SaveId or ("toggle:" .. tabTitle .. ":" .. toggleTitle), "toggle", toggleApi)
                        return toggleApi
                    end
                    sectionApi.AddSlider = function(self, sliderOpts)
                        sliderOpts = sliderOpts or {}
                        sliderOpts = wrapAutoSave(sliderOpts, makeComponentKey(sliderOpts.Title))
                        local sliderTitle = sliderOpts.Title or "Slider"
                        local minValue = sliderOpts.Min or 0
                        local maxValue = sliderOpts.Max or 100
                        local defaultValue = math.clamp(sliderOpts.Default or minValue, minValue, maxValue)
                        local callback = sliderOpts.Callback or function() end
                        local currentValue = defaultValue
                        elementOrder = elementOrder + 1
                        local sliderFrame = Instance.new("Frame")
                        sliderFrame.BackgroundColor3 = palette.Background
                        sliderFrame.BackgroundTransparency = 0.85
                        sliderFrame.Size = UDim2.new(1, 0, 0, 0)
                        sliderFrame.AutomaticSize = Enum.AutomaticSize.Y
                        sliderFrame.LayoutOrder = elementOrder
                        sliderFrame.ZIndex = 3
                        sliderFrame.Parent = tabPageScroll
                        addPadding(sliderFrame, 10, 12, 12, 12)
                        applyHoverGlow(sliderFrame, "sl_" .. sliderTitle .. elementOrder)
                        bindThemeProp(sliderFrame, "BackgroundColor3", "Background")
                        local sliderLayout = Instance.new("UIListLayout")
                        sliderLayout.FillDirection = Enum.FillDirection.Vertical
                        sliderLayout.Padding = UDim.new(0, 8)
                        sliderLayout.SortOrder = Enum.SortOrder.LayoutOrder
                        sliderLayout.Parent = sliderFrame
                        local headerRow = Instance.new("Frame")
                        headerRow.BackgroundTransparency = 1
                        headerRow.Size = UDim2.new(1, 0, 0, 18)
                        headerRow.LayoutOrder = 1
                        headerRow.ZIndex = 4
                        headerRow.Parent = sliderFrame
                        local titleLabel = Instance.new("TextLabel")
                        titleLabel.BackgroundTransparency = 1
                        titleLabel.Size = UDim2.new(1, -52, 1, 0)
                        titleLabel.FontFace = FontBold
                        titleLabel.TextSize = 13
                        titleLabel.TextColor3 = palette.TextWhite
                        titleLabel.TextTransparency = 0
                        titleLabel.TextXAlignment = Enum.TextXAlignment.Left
                        titleLabel.Text = sliderTitle
                        titleLabel.ZIndex = 5
                        titleLabel.Parent = headerRow
                        bindThemeProp(titleLabel, "TextColor3", "TextWhite")
                        local valueInputBox = Instance.new("TextBox")
                        valueInputBox.BackgroundColor3 = Color3.fromRGB(28, 28, 28)
                        valueInputBox.BackgroundTransparency = 0.3
                        valueInputBox.Size = UDim2.new(0, 42, 0, 18)
                        valueInputBox.Position = UDim2.new(1, -42, 0.5, -9)
                        valueInputBox.FontFace = FontMedium
                        valueInputBox.TextSize = 11
                        valueInputBox.TextColor3 = palette.TextWhite
                        valueInputBox.TextTransparency = 0
                        valueInputBox.Text = tostring(math.floor(currentValue))
                        valueInputBox.ClearTextOnFocus = false
                        valueInputBox.ZIndex = 5
                        valueInputBox.Parent = headerRow
                        addCorner(valueInputBox, 5)
                        bindThemeProp(valueInputBox, "TextColor3", "TextWhite")
                        local trackContainer = Instance.new("Frame")
                        trackContainer.BackgroundTransparency = 1
                        trackContainer.Size = UDim2.new(1, 0, 0, 12)
                        trackContainer.LayoutOrder = 2
                        trackContainer.ZIndex = 4
                        trackContainer.Parent = sliderFrame
                        local trackBar = Instance.new("Frame")
                        trackBar.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
                        trackBar.BackgroundTransparency = 0.2
                        trackBar.Size = UDim2.new(1, 0, 0, 4)
                        trackBar.Position = UDim2.new(0, 0, 0.5, -2)
                        trackBar.ZIndex = 4
                        trackBar.Parent = trackContainer
                        addCorner(trackBar, 2)
                        local initialRatio = (currentValue - minValue) / math.max(maxValue - minValue, 1)
                        local fillBar = Instance.new("Frame")
                        fillBar.BackgroundColor3 = palette.Accent
                        fillBar.BackgroundTransparency = 0.2
                        fillBar.Size = UDim2.new(initialRatio, 0, 1, 0)
                        fillBar.ZIndex = 5
                        fillBar.Parent = trackBar
                        addCorner(fillBar, 2)
                        onThemeChange(function()
                            fillBar.BackgroundColor3 = palette.Accent
                        end)
                        local sliderKnob = Instance.new("Frame")
                        sliderKnob.BackgroundColor3 = palette.TextWhite
                        sliderKnob.BackgroundTransparency = 0.2
                        sliderKnob.Size = UDim2.new(0, 12, 0, 12)
                        sliderKnob.Position = UDim2.new(initialRatio, -6, 0.5, -6)
                        sliderKnob.ZIndex = 6
                        sliderKnob.Parent = trackBar
                        addCorner(sliderKnob, 6)
                        local isDraggingSlider = false
                        local hoverGroupKey = "slhov_" .. sliderTitle .. elementOrder
                        sliderFrame.InputBegan:Connect(function(f0)
                            if f0.UserInputType == Enum.UserInputType.MouseMovement then
                                cancelGroupTweens(hoverGroupKey)
                                playGroupTween(hoverGroupKey, sliderFrame, TweenInfo020, {
                                    BackgroundTransparency = 0.5,
                                })
                            end
                        end)
                        sliderFrame.InputEnded:Connect(function(f0)
                            if (f0.UserInputType == Enum.UserInputType.MouseMovement) and (not isDraggingSlider) then
                                cancelGroupTweens(hoverGroupKey)
                                playGroupTween(hoverGroupKey, sliderFrame, TweenInfo020, {
                                    BackgroundTransparency = 0.85,
                                })
                            end
                        end)
                        local updateSliderFromInput = function(f0)
                            f0 = math.clamp(f0, 0, 1)
                            currentValue = math.floor((minValue + ((maxValue - minValue) * f0)) + 0.5)
                            fillBar.Size = UDim2.new(f0, 0, 1, 0)
                            sliderKnob.Position = UDim2.new(f0, -6, 0.5, -6)
                            valueInputBox.Text = tostring(currentValue)
                            callback(currentValue)
                        end
                        local sliderHitBtn = Instance.new("TextButton")
                        sliderHitBtn.BackgroundTransparency = 1
                        sliderHitBtn.Size = UDim2.new(1, 0, 1, 0)
                        sliderHitBtn.Text = ""
                        sliderHitBtn.ZIndex = 7
                        sliderHitBtn.AutoButtonColor = false
                        sliderHitBtn.Parent = trackContainer
                        sliderHitBtn.InputBegan:Connect(function(f0)
                            if (f0.UserInputType == Enum.UserInputType.MouseButton1) or (f0.UserInputType == Enum.UserInputType.Touch) then
                                isDraggingSlider = true
                                updateSliderFromInput(math.clamp((f0.Position.X - trackBar.AbsolutePosition.X) / trackBar.AbsoluteSize.X, 0, 1))
                            end
                        end)
                        table.insert(winState.connections, UserInputService.InputChanged:Connect(function(f0)
                            if isDraggingSlider and ((f0.UserInputType == Enum.UserInputType.MouseMovement) or (f0.UserInputType == Enum.UserInputType.Touch)) then
                                updateSliderFromInput(math.clamp((f0.Position.X - trackBar.AbsolutePosition.X) / trackBar.AbsoluteSize.X, 0, 1))
                            end
                        end))
                        table.insert(winState.connections, UserInputService.InputEnded:Connect(function(f0)
                            if (f0.UserInputType == Enum.UserInputType.MouseButton1) or (f0.UserInputType == Enum.UserInputType.Touch) then
                                if isDraggingSlider then
                                    playSound(SOUND_OPEN)
                                end
                                isDraggingSlider = false
                            end
                        end))
                        valueInputBox.FocusLost:Connect(function()
                            local f0 = tonumber(valueInputBox.Text)
                            if f0 then
                                updateSliderFromInput((math.clamp(math.floor(f0), minValue, maxValue) - minValue) / math.max(maxValue - minValue, 1))
                            else
                                valueInputBox.Text = tostring(currentValue)
                            end
                        end)
                        local sliderApi = {
                            Set = function(f0, f1)
                                f1 = math.clamp(f1, minValue, maxValue)
                                updateSliderFromInput((f1 - minValue) / math.max(maxValue - minValue, 1))
                            end,
                            Get = function(f0)
                                return currentValue
                            end,
                            GetFrame = function(f0)
                                return sliderFrame
                            end,
                        }
                        registerSearchItem(sliderTitle, "", sliderFrame)
                        return sliderApi
                    end
                    sectionApi.AddButton = function(self, buttonOpts)
                        buttonOpts = buttonOpts or {}
                        local buttonTitle = buttonOpts.Title or "Button"
                        local buttonDesc = buttonOpts.Description or ""
                        local buttonIcon = Lucide.Resolve(buttonOpts.Icon, "rbxassetid://134116239949429")
                        local callback = buttonOpts.Callback or function() end
                        local requireConfirm = buttonOpts.Confirmation or false
                        elementOrder = elementOrder + 1
                        local buttonFrame = Instance.new("TextButton")
                        buttonFrame.BackgroundColor3 = palette.Background
                        buttonFrame.BackgroundTransparency = 0.85
                        buttonFrame.Size = UDim2.new(1, 0, 0, 0)
                        buttonFrame.AutomaticSize = Enum.AutomaticSize.Y
                        buttonFrame.AutoButtonColor = false
                        buttonFrame.Text = ""
                        buttonFrame.LayoutOrder = elementOrder
                        buttonFrame.ZIndex = 3
                        buttonFrame.Parent = tabPageScroll
                        addPadding(buttonFrame, 10, 12, 10, 12)
                        applyHoverGlow(buttonFrame, "btn_" .. buttonTitle .. elementOrder)
                        bindThemeProp(buttonFrame, "BackgroundColor3", "Background")
                        local textLayout = Instance.new("UIListLayout")
                        textLayout.FillDirection = Enum.FillDirection.Vertical
                        textLayout.Padding = UDim.new(0, 1)
                        textLayout.SortOrder = Enum.SortOrder.LayoutOrder
                        textLayout.Parent = buttonFrame
                        local textContainer = Instance.new("Frame")
                        textContainer.BackgroundTransparency = 1
                        textContainer.Size = UDim2.new(1, 0, 0, 18)
                        textContainer.LayoutOrder = 1
                        textContainer.ZIndex = 4
                        textContainer.Parent = buttonFrame
                        local titleLabel = Instance.new("TextLabel")
                        titleLabel.BackgroundTransparency = 1
                        titleLabel.Size = UDim2.new(1, -44, 1, 0)
                        titleLabel.FontFace = FontBold
                        titleLabel.TextSize = 13
                        titleLabel.TextColor3 = palette.TextWhite
                        titleLabel.TextXAlignment = Enum.TextXAlignment.Left
                        titleLabel.Text = buttonTitle
                        titleLabel.ZIndex = 5
                        titleLabel.Parent = textContainer
                        bindThemeProp(titleLabel, "TextColor3", "TextWhite")
                        if buttonDesc ~= "" then
                            local e11 = Instance.new("TextLabel")
                            e11.BackgroundTransparency = 1
                            e11.Size = UDim2.new(1, 0, 0, 0)
                            e11.AutomaticSize = Enum.AutomaticSize.Y
                            e11.FontFace = FontMedium
                            e11.TextSize = 11
                            e11.TextColor3 = palette.TextSubtitle
                            e11.TextXAlignment = Enum.TextXAlignment.Left
                            e11.TextWrapped = true
                            e11.Text = buttonDesc
                            e11.LayoutOrder = 2
                            e11.ZIndex = 5
                            e11.RichText = true
                            e11.Parent = buttonFrame
                            bindThemeProp(e11, "TextColor3", "TextSubtitle")
                        end
                        local iconImage = Instance.new("ImageLabel")
                        iconImage.BackgroundTransparency = 1
                        iconImage.Size = UDim2.new(0, 20, 0, 20)
                        iconImage.AnchorPoint = Vector2.new(1, 0.5)
                        iconImage.Position = UDim2.new(1, 0, 0.5, 0)
                        iconImage.Image = buttonIcon
                        iconImage.ImageColor3 = palette.Accent
                        iconImage.ImageTransparency = 0.2
                        iconImage.ZIndex = 5
                        iconImage.Parent = textContainer
                        onThemeChange(function()
                            iconImage.ImageColor3 = palette.Accent
                        end)
                        local hoverGroupKey = "btnhov_" .. buttonTitle .. elementOrder
                        buttonFrame.MouseEnter:Connect(function()
                            cancelGroupTweens(hoverGroupKey)
                            playGroupTween(hoverGroupKey, buttonFrame, TweenInfo020, {
                                BackgroundTransparency = 0.5,
                            })
                            playGroupTween(hoverGroupKey, iconImage, TweenInfo020, {
                                ImageTransparency = 0,
                                Size = UDim2.new(0, 23, 0, 23),
                            })
                        end)
                        buttonFrame.MouseLeave:Connect(function()
                            cancelGroupTweens(hoverGroupKey)
                            playGroupTween(hoverGroupKey, buttonFrame, TweenInfo020, {
                                BackgroundTransparency = 0.85,
                            })
                            playGroupTween(hoverGroupKey, iconImage, TweenInfo020, {
                                ImageTransparency = 0.2,
                                Size = UDim2.new(0, 20, 0, 20),
                            })
                        end)
                        local triggerButton = function()
                            local f0 = "btncl_" .. buttonTitle .. elementOrder
                            cancelGroupTweens(f0)
                            playSound(SOUND_OPEN)
                            playGroupTween(f0, buttonFrame, TweenInfo.new(0.07, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
                                BackgroundTransparency = 0.2,
                            })
                            playGroupTween(f0, iconImage, TweenInfo.new(0.07, Enum.EasingStyle.Quad, Enum.EasingDirection.Out), {
                                ImageColor3 = palette.AccentBright,
                            })
                            task.delay(0.14, function()
                                cancelGroupTweens(f0)
                                playGroupTween(f0, buttonFrame, TweenInfo035, {
                                    BackgroundTransparency = 0.85,
                                })
                                playGroupTween(f0, iconImage, TweenInfo035, {
                                    ImageColor3 = palette.Accent,
                                })
                            end)
                            callback()
                        end
                        buttonFrame.MouseButton1Click:Connect(function()
                            if winState.destroyed then
                                return
                            end
                            if requireConfirm then
                                showConfirmDialog("Do you want to execute this action?", "dialog_btn" .. elementOrder, function()
                                    triggerButton()
                                end)
                            else
                                triggerButton()
                            end
                        end)
                        local buttonApi = {
                            GetFrame = function(f0)
                                return buttonFrame
                            end,
                            SetTitle = function(f0, f1)
                                titleLabel.Text = f1
                            end,
                        }
                        registerSearchItem(buttonTitle, buttonDesc, buttonFrame)
                        return buttonApi
                    end
                    sectionApi.AddDropdown = function(self, dropdownOpts)
                        dropdownOpts = dropdownOpts or {}
                        dropdownOpts = wrapAutoSave(dropdownOpts, makeComponentKey(dropdownOpts.Title))
                        local dropdownTitle = dropdownOpts.Title or "Dropdown"
                        local optionList = ((dropdownOpts.Options or dropdownOpts.Values) or dropdownOpts.List) or {}
                        local isMultiSelect = (dropdownOpts.Multiple or dropdownOpts.Multi) or false
                        local defaultSelection = dropdownOpts.Default
                        if defaultSelection == nil then
                            defaultSelection = {}
                        elseif type(defaultSelection) ~= "table" then
                            defaultSelection = {
                                defaultSelection,
                            }
                        end
                        local callback = dropdownOpts.Callback or function() end
                        elementOrder = elementOrder + 1
                        local selectedMap = {}
                        if isMultiSelect then
                            for e11, e12 in ipairs(defaultSelection) do
                                selectedMap[tostring(e12)] = true
                            end
                        elseif defaultSelection[1] then
                            selectedMap[tostring(defaultSelection[1])] = true
                        end
                        local isOpen = false
                        local dropdownContainer = Instance.new("Frame")
                        dropdownContainer.BackgroundTransparency = 1
                        dropdownContainer.Size = UDim2.new(1, 0, 0, 0)
                        dropdownContainer.AutomaticSize = Enum.AutomaticSize.Y
                        dropdownContainer.LayoutOrder = elementOrder
                        dropdownContainer.ZIndex = 3
                        dropdownContainer.Parent = tabPageScroll
                        local dropdownLayout = Instance.new("UIListLayout")
                        dropdownLayout.FillDirection = Enum.FillDirection.Vertical
                        dropdownLayout.Padding = UDim.new(0, 4)
                        dropdownLayout.SortOrder = Enum.SortOrder.LayoutOrder
                        dropdownLayout.Parent = dropdownContainer
                        local headerFrame = Instance.new("Frame")
                        headerFrame.BackgroundColor3 = palette.Background
                        headerFrame.BackgroundTransparency = 0.85
                        headerFrame.Size = UDim2.new(1, 0, 0, 40)
                        headerFrame.LayoutOrder = 1
                        headerFrame.ZIndex = 4
                        headerFrame.Parent = dropdownContainer
                        addPadding(headerFrame, 6, 12, 6, 12)
                        applyHoverGlow(headerFrame, "dd_" .. dropdownTitle .. elementOrder)
                        bindThemeProp(headerFrame, "BackgroundColor3", "Background")
                        local titleRow = Instance.new("Frame")
                        titleRow.BackgroundTransparency = 1
                        titleRow.Size = UDim2.new(1, 0, 1, 0)
                        titleRow.ZIndex = 5
                        titleRow.Parent = headerFrame
                        local titleLabel = Instance.new("TextLabel")
                        titleLabel.BackgroundTransparency = 1
                        titleLabel.Size = UDim2.new(1, -22, 0, 16)
                        titleLabel.Position = UDim2.new(0, 0, 0, 0)
                        titleLabel.FontFace = FontBold
                        titleLabel.TextSize = 13
                        titleLabel.TextColor3 = palette.TextWhite
                        titleLabel.TextXAlignment = Enum.TextXAlignment.Left
                        titleLabel.Text = dropdownTitle
                        titleLabel.ZIndex = 6
                        titleLabel.Parent = titleRow
                        bindThemeProp(titleLabel, "TextColor3", "TextWhite")
                        local getSelectedSummary = function()
                            local f0 = {}
                            for f4, f5 in ipairs(optionList) do
                                local f6 = ((type(f5) == "table") and tostring(f5.Value or f5[1])) or tostring(f5)
                                if selectedMap[f6] then
                                    table.insert(f0, f6)
                                end
                            end
                            return ((#f0 > 0) and table.concat(f0, ", ")) or "None"
                        end
                        local selectedSummaryLabel = Instance.new("TextLabel")
                        selectedSummaryLabel.BackgroundTransparency = 1
                        selectedSummaryLabel.Size = UDim2.new(1, -22, 0, 12)
                        selectedSummaryLabel.Position = UDim2.new(0, 0, 0, 16)
                        selectedSummaryLabel.FontFace = FontMedium
                        selectedSummaryLabel.TextSize = 10
                        selectedSummaryLabel.TextColor3 = palette.TextSubtitle
                        selectedSummaryLabel.TextXAlignment = Enum.TextXAlignment.Left
                        selectedSummaryLabel.Text = getSelectedSummary()
                        selectedSummaryLabel.ZIndex = 6
                        selectedSummaryLabel.Parent = titleRow
                        bindThemeProp(selectedSummaryLabel, "TextColor3", "TextSubtitle")
                        local arrowIcon = Instance.new("ImageLabel")
                        arrowIcon.BackgroundTransparency = 1
                        arrowIcon.Size = UDim2.new(0, 14, 0, 14)
                        arrowIcon.AnchorPoint = Vector2.new(1, 0.5)
                        arrowIcon.Position = UDim2.new(1, 0, 0.5, 0)
                        arrowIcon.Image = "rbxassetid://10709790948"
                        arrowIcon.Rotation = 0
                        arrowIcon.ImageColor3 = palette.TextSubtitle
                        arrowIcon.ZIndex = 6
                        arrowIcon.Parent = titleRow
                        bindThemeProp(arrowIcon, "ImageColor3", "TextSubtitle")
                        local drawerClipFrame = Instance.new("Frame")
                        drawerClipFrame.BackgroundTransparency = 1
                        drawerClipFrame.Size = UDim2.new(1, 0, 0, 0)
                        drawerClipFrame.ClipsDescendants = true
                        drawerClipFrame.LayoutOrder = 2
                        drawerClipFrame.ZIndex = 20
                        drawerClipFrame.Parent = dropdownContainer
                        local searchBarFrame = Instance.new("Frame")
                        searchBarFrame.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
                        searchBarFrame.BackgroundTransparency = 0.2
                        searchBarFrame.Size = UDim2.new(1, 0, 0, 26)
                        searchBarFrame.Position = UDim2.new(0, 0, 0, 0)
                        searchBarFrame.ZIndex = 20
                        searchBarFrame.Parent = drawerClipFrame
                        addCorner(searchBarFrame, 6)
                        local searchIcon = Instance.new("ImageLabel")
                        searchIcon.BackgroundTransparency = 1
                        searchIcon.Size = UDim2.new(0, 12, 0, 12)
                        searchIcon.Position = UDim2.new(0, 8, 0.5, -6)
                        searchIcon.Image = "rbxassetid://115739298989740"
                        searchIcon.ImageColor3 = palette.TextSubtitle
                        searchIcon.ZIndex = 21
                        searchIcon.Parent = searchBarFrame
                        bindThemeProp(searchIcon, "ImageColor3", "TextSubtitle")
                        local searchBox = Instance.new("TextBox")
                        searchBox.BackgroundTransparency = 1
                        searchBox.Size = UDim2.new(1, -30, 1, 0)
                        searchBox.Position = UDim2.new(0, 26, 0, 0)
                        searchBox.FontFace = FontMedium
                        searchBox.TextSize = 11
                        searchBox.TextColor3 = palette.TextWhite
                        searchBox.PlaceholderColor3 = palette.TextSubtitle
                        searchBox.PlaceholderText = "Search..."
                        searchBox.TextXAlignment = Enum.TextXAlignment.Left
                        searchBox.ClearTextOnFocus = false
                        searchBox.Text = ""
                        searchBox.ZIndex = 21
                        searchBox.Parent = searchBarFrame
                        bindThemeProp(searchBox, "TextColor3", "TextWhite")
                        bindThemeProp(searchBox, "PlaceholderColor3", "TextSubtitle")
                        local optionsScroll = Instance.new("ScrollingFrame")
                        optionsScroll.BackgroundColor3 = Color3.fromRGB(15, 15, 15)
                        optionsScroll.Size = UDim2.new(1, 0, 1, -30)
                        optionsScroll.Position = UDim2.new(0, 0, 0, 30)
                        optionsScroll.CanvasSize = UDim2.new(0, 0, 0, 0)
                        optionsScroll.AutomaticCanvasSize = Enum.AutomaticSize.Y
                        optionsScroll.ScrollBarThickness = 2
                        optionsScroll.ScrollBarImageColor3 = MutedTextColor
                        optionsScroll.ZIndex = 20
                        optionsScroll.Parent = drawerClipFrame
                        optionsScroll.BorderSizePixel = 0
                        addCorner(optionsScroll, 8)
                        local optionsStroke = addStroke(optionsScroll, palette.Border, 1, 0.45)
                        onThemeChange(function()
                            optionsStroke.Color = palette.Border
                        end)
                        local optionsListLayout = Instance.new("UIListLayout")
                        optionsListLayout.FillDirection = Enum.FillDirection.Vertical
                        optionsListLayout.Padding = UDim.new(0, 5)
                        optionsListLayout.SortOrder = Enum.SortOrder.LayoutOrder
                        optionsListLayout.Parent = optionsScroll
                        addPadding(optionsScroll, 5, 5, 5, 5)
                        local optionRows = {}
                        searchBox:GetPropertyChangedSignal("Text"):Connect(function()
                            local f0 = searchBox.Text:lower()
                            for f4, f5 in ipairs(optionRows) do
                                f5._frame.Visible = (f0 == "") or (f5._val:lower():find(f0, 1, true) ~= nil)
                            end
                        end)
                        local refreshOptionVisuals = function()
                            selectedSummaryLabel.Text = getSelectedSummary()
                            for f3, f4 in ipairs(optionRows) do
                                local f5 = selectedMap[f4._val] == true
                                TweenService:Create(f4._bar, TweenInfo020, {
                                    BackgroundTransparency = (f5 and 0) or 1,
                                }):Play()
                                TweenService:Create(f4._frame, TweenInfo020, {
                                    BackgroundTransparency = (f5 and 0.82) or 1,
                                    BackgroundColor3 = palette.Background,
                                }):Play()
                                TweenService:Create(f4._lbl, TweenInfo020, {
                                    TextColor3 = (f5 and palette.AccentBright) or palette.TextWhite,
                                }):Play()
                            end
                        end
                        local calcDrawerHeight = function()
                            local f0 = 40
                            for f4, f5 in ipairs(optionList) do
                                f0 = f0 + ((((((type(f5) == "table") and (f5.Description or "")) or "") ~= "") and 41) or 29)
                            end
                            return math.min(f0, 190)
                        end
                        for e30, e31 in ipairs(optionList) do
                            local e32 = ((type(e31) == "table") and tostring(e31.Value or e31[1])) or tostring(e31)
                            local e33 = ((type(e31) == "table") and (e31.Description or "")) or ""
                            local e34 = selectedMap[e32] == true
                            local e35 = ((e33 ~= "") and 36) or 24
                            local e36 = Instance.new("Frame")
                            e36.BackgroundColor3 = palette.Background
                            e36.BackgroundTransparency = (e34 and 0.82) or 1
                            e36.Size = UDim2.new(1, 0, 0, 0)
                            e36.AutomaticSize = Enum.AutomaticSize.Y
                            e36.LayoutOrder = e30
                            e36.ZIndex = 21
                            e36.Parent = optionsScroll
                            addCorner(e36, 5)
                            bindThemeProp(e36, "BackgroundColor3", "Background")
                            local e37 = Instance.new("Frame")
                            e37.BackgroundColor3 = palette.Accent
                            e37.BackgroundTransparency = (e34 and 0) or 1
                            e37.Size = UDim2.new(0, 2, 0, 20)
                            e37.Position = UDim2.new(0, 1, 0, 5)
                            e37.ZIndex = 22
                            e37.Parent = e36
                            addCorner(e37, 1)
                            onThemeChange(function()
                                e37.BackgroundColor3 = palette.Accent
                            end)
                            local e38 = Instance.new("TextLabel")
                            e38.BackgroundTransparency = 1
                            e38.Size = UDim2.new(1, -14, 0, 13)
                            e38.Position = UDim2.new(0, 10, 0, 5)
                            e38.FontFace = FontBold
                            e38.TextSize = 10
                            e38.TextColor3 = (e34 and palette.AccentBright) or palette.TextWhite
                            e38.TextXAlignment = Enum.TextXAlignment.Left
                            e38.Text = e32
                            e38.ZIndex = 22
                            e38.Parent = e36
                            bindThemeProp(e38, "TextColor3", "TextWhite")
                            if e33 ~= "" then
                                local e39 = Instance.new("TextLabel")
                                e39.BackgroundTransparency = 1
                                e39.Size = UDim2.new(1, -14, 0, 0)
                                e39.AutomaticSize = Enum.AutomaticSize.Y
                                e39.Position = UDim2.new(0, 10, 0, 17)
                                e39.FontFace = FontMedium
                                e39.TextSize = 9
                                e39.TextColor3 = palette.TextSubtitle
                                e39.TextXAlignment = Enum.TextXAlignment.Left
                                e39.TextWrapped = true
                                e39.Text = e33
                                e39.ZIndex = 22
                                e39.Parent = e36
                            end
                            local e39 = Instance.new("TextButton")
                            e39.BackgroundTransparency = 1
                            e39.Size = UDim2.new(1, 0, 1, 0)
                            e39.Text = ""
                            e39.ZIndex = 23
                            e39.AutoButtonColor = false
                            e39.Parent = e36
                            local e40 = "ddopt_" .. e32 .. elementOrder
                            e39.MouseEnter:Connect(function()
                                if not selectedMap[e32] then
                                    cancelGroupTweens(e40)
                                    playGroupTween(e40, e36, TweenInfo020, {
                                        BackgroundColor3 = palette.Background,
                                        BackgroundTransparency = 0.88,
                                    })
                                end
                            end)
                            e39.MouseLeave:Connect(function()
                                if not selectedMap[e32] then
                                    cancelGroupTweens(e40)
                                    playGroupTween(e40, e36, TweenInfo020, {
                                        BackgroundColor3 = palette.Background,
                                        BackgroundTransparency = 1,
                                    })
                                end
                            end)
                            e39.MouseButton1Click:Connect(function()
                                playSound(SOUND_OPEN)
                                if isMultiSelect then
                                    selectedMap[e32] = not selectedMap[e32]
                                else
                                    if selectedMap[e32] then
                                        return
                                    end
                                    for f3 in pairs(selectedMap) do
                                        selectedMap[f3] = false
                                    end
                                    selectedMap[e32] = true
                                end
                                local f0 = {}
                                for f4, f5 in ipairs(optionList) do
                                    local f6 = ((type(f5) == "table") and tostring(f5.Value or f5[1])) or tostring(f5)
                                    if selectedMap[f6] then
                                        table.insert(f0, f6)
                                    end
                                end
                                refreshOptionVisuals()
                                callback((isMultiSelect and f0) or f0[1])
                            end)
                            table.insert(optionRows, {
                                _frame = e36,
                                _bar = e37,
                                _val = e32,
                                _lbl = e38,
                            })
                        end
                        onThemeChange(function()
                            for f3, f4 in ipairs(optionRows) do
                                f4._bar.BackgroundColor3 = palette.Accent
                                f4._lbl.TextColor3 = (selectedMap[f4._val] and palette.AccentBright) or palette.TextWhite
                            end
                        end)
                        local drawerTargetHeight = calcDrawerHeight()
                        local openDropdown = function()
                            isOpen = true
                            cancelGroupTweens("ddmenu_" .. elementOrder)
                            playGroupTween("ddmenu_" .. elementOrder, drawerClipFrame, TweenInfo035, {
                                Size = UDim2.new(1, 0, 0, drawerTargetHeight),
                            })
                            playGroupTween("ddmenu_" .. elementOrder, headerFrame, TweenInfo020, {
                                BackgroundTransparency = 0.7,
                            })
                            playGroupTween("ddmenu_" .. elementOrder, arrowIcon, TweenInfo020, {
                                Rotation = 180,
                            })
                        end
                        local closeDropdown = function()
                            isOpen = false
                            cancelGroupTweens("ddmenu_" .. elementOrder)
                            playGroupTween("ddmenu_" .. elementOrder, drawerClipFrame, TweenInfo020, {
                                Size = UDim2.new(1, 0, 0, 0),
                            })
                            playGroupTween("ddmenu_" .. elementOrder, headerFrame, TweenInfo020, {
                                BackgroundTransparency = 0.85,
                            })
                            playGroupTween("ddmenu_" .. elementOrder, arrowIcon, TweenInfo020, {
                                Rotation = 0,
                            })
                            searchBox.Text = ""
                        end
                        local hoverGroupKey = "ddhov_" .. dropdownTitle .. elementOrder
                        headerFrame.InputBegan:Connect(function(f0)
                            if f0.UserInputType == Enum.UserInputType.MouseMovement then
                                cancelGroupTweens(hoverGroupKey)
                                if not isOpen then
                                    playGroupTween(hoverGroupKey, headerFrame, TweenInfo020, {
                                        BackgroundTransparency = 0.5,
                                    })
                                end
                            end
                        end)
                        headerFrame.InputEnded:Connect(function(f0)
                            if f0.UserInputType == Enum.UserInputType.MouseMovement then
                                cancelGroupTweens(hoverGroupKey)
                                if not isOpen then
                                    playGroupTween(hoverGroupKey, headerFrame, TweenInfo020, {
                                        BackgroundTransparency = 0.85,
                                    })
                                end
                            end
                        end)
                        local headerToggleBtn = Instance.new("TextButton")
                        headerToggleBtn.BackgroundTransparency = 1
                        headerToggleBtn.Size = UDim2.new(1, 0, 1, 0)
                        headerToggleBtn.Text = ""
                        headerToggleBtn.ZIndex = 7
                        headerToggleBtn.AutoButtonColor = false
                        headerToggleBtn.Parent = headerFrame
                        headerToggleBtn.MouseButton1Click:Connect(function()
                            if isOpen then
                                closeDropdown()
                            else
                                openDropdown()
                            end
                        end)
                        local dropdownApi = {
                            Set = function(f0, f1)
                                if isMultiSelect and (type(f1) == "table") then
                                    for f5 in pairs(selectedMap) do
                                        selectedMap[f5] = false
                                    end
                                    for f5, f6 in ipairs(f1) do
                                        selectedMap[tostring(f6)] = true
                                    end
                                else
                                    for f5 in pairs(selectedMap) do
                                        selectedMap[f5] = false
                                    end
                                    selectedMap[tostring(f1)] = true
                                end
                                refreshOptionVisuals()
                            end,
                            Get = function(f0)
                                local f1 = {}
                                for f5, f6 in ipairs(optionList) do
                                    local f7 = ((type(f6) == "table") and tostring(f6.Value or f6[1])) or tostring(f6)
                                    if selectedMap[f7] then
                                        table.insert(f1, f7)
                                    end
                                end
                                return (isMultiSelect and f1) or f1[1]
                            end,
                            Close = function(f0)
                                closeDropdown()
                            end,
                            Open = function(f0)
                                openDropdown()
                            end,
                            GetFrame = function(f0)
                                return dropdownContainer
                            end,
                            SetTitle = function(f0, f1)
                                titleLabel.Text = f1
                            end,
                            Refresh = function(f0, f1)
                                closeDropdown()
                                for f5, f6 in ipairs(optionRows) do
                                    f6._frame:Destroy()
                                end
                                optionRows = {}
                                for f5 in pairs(selectedMap) do
                                    selectedMap[f5] = false
                                end
                                optionList = f1 or {}
                                for f5, f6 in ipairs(optionList) do
                                    local f7 = ((type(f6) == "table") and tostring(f6.Value or f6[1])) or tostring(f6)
                                    local f8 = ((type(f6) == "table") and (f6.Description or "")) or ""
                                    local f9 = ((f8 ~= "") and 36) or 24
                                    local f10 = Instance.new("Frame")
                                    f10.BackgroundColor3 = palette.Background
                                    f10.BackgroundTransparency = 1
                                    f10.Size = UDim2.new(1, 0, 0, 0)
                                    f10.AutomaticSize = Enum.AutomaticSize.Y
                                    f10.LayoutOrder = f5
                                    f10.ZIndex = 21
                                    f10.Parent = optionsScroll
                                    addCorner(f10, 5)
                                    bindThemeProp(f10, "BackgroundColor3", "Background")
                                    local f11 = Instance.new("Frame")
                                    f11.BackgroundColor3 = palette.Accent
                                    f11.BackgroundTransparency = 1
                                    f11.Size = UDim2.new(0, 2, 0, 20)
                                    f11.Position = UDim2.new(0, 1, 0, 5)
                                    f11.ZIndex = 22
                                    f11.Parent = f10
                                    addCorner(f11, 1)
                                    onThemeChange(function()
                                        f11.BackgroundColor3 = palette.Accent
                                    end)
                                    local f12 = Instance.new("TextLabel")
                                    f12.BackgroundTransparency = 1
                                    f12.Size = UDim2.new(1, -14, 0, 13)
                                    f12.Position = UDim2.new(0, 10, 0, 5)
                                    f12.FontFace = FontBold
                                    f12.TextSize = 10
                                    f12.TextColor3 = palette.TextWhite
                                    f12.TextXAlignment = Enum.TextXAlignment.Left
                                    f12.Text = f7
                                    f12.ZIndex = 22
                                    f12.Parent = f10
                                    bindThemeProp(f12, "TextColor3", "TextWhite")
                                    if f8 ~= "" then
                                        local f13 = Instance.new("TextLabel")
                                        f13.BackgroundTransparency = 1
                                        f13.Size = UDim2.new(1, -14, 0, 0)
                                        f13.AutomaticSize = Enum.AutomaticSize.Y
                                        f13.Position = UDim2.new(0, 10, 0, 17)
                                        f13.FontFace = FontMedium
                                        f13.TextSize = 9
                                        f13.TextColor3 = palette.TextSubtitle
                                        f13.TextXAlignment = Enum.TextXAlignment.Left
                                        f13.TextWrapped = true
                                        f13.Text = f8
                                        f13.ZIndex = 22
                                        f13.Parent = f10
                                    end
                                    local f13 = Instance.new("TextButton")
                                    f13.BackgroundTransparency = 1
                                    f13.Size = UDim2.new(1, 0, 1, 0)
                                    f13.Text = ""
                                    f13.ZIndex = 23
                                    f13.AutoButtonColor = false
                                    f13.Parent = f10
                                    local f14 = "ddopt_" .. f7 .. elementOrder
                                    f13.MouseEnter:Connect(function()
                                        if not selectedMap[f7] then
                                            cancelGroupTweens(f14)
                                            playGroupTween(f14, f10, TweenInfo020, {
                                                BackgroundColor3 = palette.Background,
                                                BackgroundTransparency = 0.88,
                                            })
                                        end
                                    end)
                                    f13.MouseLeave:Connect(function()
                                        if not selectedMap[f7] then
                                            cancelGroupTweens(f14)
                                            playGroupTween(f14, f10, TweenInfo020, {
                                                BackgroundColor3 = palette.Background,
                                                BackgroundTransparency = 1,
                                            })
                                        end
                                    end)
                                    f13.MouseButton1Click:Connect(function()
                                        playSound(SOUND_OPEN)
                                        if isMultiSelect then
                                            selectedMap[f7] = not selectedMap[f7]
                                        else
                                            if selectedMap[f7] then
                                                return
                                            end
                                            for g3 in pairs(selectedMap) do
                                                selectedMap[g3] = false
                                            end
                                            selectedMap[f7] = true
                                        end
                                        local g0 = {}
                                        for g4, g5 in ipairs(optionList) do
                                            local g6 = ((type(g5) == "table") and tostring(g5.Value or g5[1])) or tostring(g5)
                                            if selectedMap[g6] then
                                                table.insert(g0, g6)
                                            end
                                        end
                                        refreshOptionVisuals()
                                        callback((isMultiSelect and g0) or g0[1])
                                    end)
                                    table.insert(optionRows, {
                                        _frame = f10,
                                        _bar = f11,
                                        _val = f7,
                                        _lbl = f12,
                                    })
                                end
                                drawerTargetHeight = calcDrawerHeight()
                                selectedSummaryLabel.Text = getSelectedSummary()
                            end,
                        }
                        if defaultSelection[1] ~= nil then
                            task.defer(function()
                                local f0 = {}
                                for f4, f5 in ipairs(optionList) do
                                    local f6 = ((type(f5) == "table") and tostring(f5.Value or f5[1])) or tostring(f5)
                                    if selectedMap[f6] then
                                        table.insert(f0, f6)
                                    end
                                end
                                callback((isMultiSelect and f0) or f0[1])
                            end)
                        end
                        registerSearchItem(dropdownTitle, "", dropdownContainer)
                        return dropdownApi
                    end
                    sectionApi.AddInput = function(self, inputOpts)
                        inputOpts = inputOpts or {}
                        inputOpts = wrapAutoSave(inputOpts, makeComponentKey(inputOpts.Title))
                        local inputTitle = inputOpts.Title or "Text"
                        local placeholderText = (inputOpts.PlaceHolder or inputOpts.Placeholder) or "Type here..."
                        local maxLength = inputOpts.MaxLength or 200
                        local callback = inputOpts.Callback or function() end
                        local defaultText = inputOpts.Default or ""
                        elementOrder = elementOrder + 1
                        local inputContainer = Instance.new("Frame")
                        inputContainer.BackgroundColor3 = palette.Background
                        inputContainer.BackgroundTransparency = 0.85
                        inputContainer.Size = UDim2.new(1, 0, 0, 0)
                        inputContainer.AutomaticSize = Enum.AutomaticSize.Y
                        inputContainer.LayoutOrder = elementOrder
                        inputContainer.ZIndex = 3
                        inputContainer.Parent = tabPageScroll
                        addPadding(inputContainer, 10, 12, 12, 12)
                        applyHoverGlow(inputContainer, "tb_" .. inputTitle .. elementOrder)
                        bindThemeProp(inputContainer, "BackgroundColor3", "Background")
                        local inputLayout = Instance.new("UIListLayout")
                        inputLayout.FillDirection = Enum.FillDirection.Vertical
                        inputLayout.Padding = UDim.new(0, 8)
                        inputLayout.SortOrder = Enum.SortOrder.LayoutOrder
                        inputLayout.Parent = inputContainer
                        local headerRow = Instance.new("Frame")
                        headerRow.BackgroundTransparency = 1
                        headerRow.Size = UDim2.new(1, 0, 0, 16)
                        headerRow.LayoutOrder = 1
                        headerRow.ZIndex = 4
                        headerRow.Parent = inputContainer
                        local titleLabel = Instance.new("TextLabel")
                        titleLabel.BackgroundTransparency = 1
                        titleLabel.Size = UDim2.new(1, -50, 1, 0)
                        titleLabel.FontFace = FontBold
                        titleLabel.TextSize = 13
                        titleLabel.TextColor3 = palette.TextWhite
                        titleLabel.TextTransparency = 0
                        titleLabel.TextXAlignment = Enum.TextXAlignment.Left
                        titleLabel.Text = inputTitle
                        titleLabel.ZIndex = 5
                        titleLabel.Parent = headerRow
                        bindThemeProp(titleLabel, "TextColor3", "TextWhite")
                        local charCountLabel = Instance.new("TextLabel")
                        charCountLabel.BackgroundTransparency = 1
                        charCountLabel.Size = UDim2.new(0, 46, 1, 0)
                        charCountLabel.Position = UDim2.new(1, -46, 0, 0)
                        charCountLabel.FontFace = FontMedium
                        charCountLabel.TextSize = 10
                        charCountLabel.TextColor3 = palette.TextSubtitle
                        charCountLabel.TextTransparency = 0.3
                        charCountLabel.TextXAlignment = Enum.TextXAlignment.Right
                        charCountLabel.Text = "0/" .. maxLength
                        charCountLabel.ZIndex = 5
                        charCountLabel.Parent = headerRow
                        bindThemeProp(charCountLabel, "TextColor3", "TextSubtitle")
                        local boxOuterFrame = Instance.new("Frame")
                        boxOuterFrame.BackgroundTransparency = 1
                        boxOuterFrame.Size = UDim2.new(1, 0, 0, 22)
                        boxOuterFrame.LayoutOrder = 2
                        boxOuterFrame.ZIndex = 4
                        boxOuterFrame.Parent = inputContainer
                        local boxInnerFrame = Instance.new("Frame")
                        boxInnerFrame.BackgroundColor3 = palette.Border
                        boxInnerFrame.BackgroundTransparency = 0.3
                        boxInnerFrame.Size = UDim2.new(1, 0, 0, 1)
                        boxInnerFrame.Position = UDim2.new(0, 0, 1, -1)
                        boxInnerFrame.BorderSizePixel = 0
                        boxInnerFrame.ZIndex = 4
                        boxInnerFrame.Parent = boxOuterFrame
                        bindThemeProp(boxInnerFrame, "BackgroundColor3", "Border")
                        local focusBarBg = Instance.new("Frame")
                        focusBarBg.BackgroundColor3 = palette.Accent
                        focusBarBg.BackgroundTransparency = 1
                        focusBarBg.Size = UDim2.new(0, 0, 1, 0)
                        focusBarBg.BorderSizePixel = 0
                        focusBarBg.ZIndex = 5
                        focusBarBg.Parent = boxInnerFrame
                        onThemeChange(function()
                            focusBarBg.BackgroundColor3 = palette.Accent
                        end)
                        local focusBarFill = Instance.new("Frame")
                        focusBarFill.BackgroundTransparency = 1
                        focusBarFill.Size = UDim2.new(1, 0, 0, 18)
                        focusBarFill.Position = UDim2.new(0, 0, 0, 0)
                        focusBarFill.ClipsDescendants = true
                        focusBarFill.ZIndex = 5
                        focusBarFill.Parent = boxOuterFrame
                        local textBox = Instance.new("TextBox")
                        textBox.BackgroundTransparency = 1
                        textBox.Size = UDim2.new(1, 0, 1, 0)
                        textBox.FontFace = FontMedium
                        textBox.TextSize = 12
                        textBox.TextColor3 = palette.TextWhite
                        textBox.PlaceholderColor3 = palette.TextSubtitle
                        textBox.PlaceholderText = placeholderText
                        textBox.TextXAlignment = Enum.TextXAlignment.Left
                        textBox.Text = defaultText
                        textBox.ClearTextOnFocus = false
                        textBox.TextTruncate = Enum.TextTruncate.AtEnd
                        textBox.ZIndex = 6
                        textBox.Parent = focusBarFill
                        bindThemeProp(textBox, "TextColor3", "TextWhite")
                        bindThemeProp(textBox, "PlaceholderColor3", "TextSubtitle")
                        charCountLabel.Text = #defaultText .. "/" .. maxLength
                        local isFocused = false
                        local onFocusEffect = function()
                            isFocused = true
                            cancelGroupTweens("tb_focus_" .. elementOrder)
                            playGroupTween("tb_focus_" .. elementOrder, focusBarBg, TweenInfo035, {
                                Size = UDim2.new(1, 0, 1, 0),
                                BackgroundTransparency = 0,
                            })
                            playGroupTween("tb_focus_" .. elementOrder, titleLabel, TweenInfo020, {
                                TextColor3 = palette.AccentBright,
                                TextTransparency = 0,
                            })
                            playGroupTween("tb_focus_" .. elementOrder, charCountLabel, TweenInfo020, {
                                TextTransparency = 0,
                            })
                            playGroupTween("tb_focus_" .. elementOrder, inputContainer, TweenInfo020, {
                                BackgroundTransparency = 0.5,
                            })
                        end
                        local onBlurEffect = function()
                            isFocused = false
                            cancelGroupTweens("tb_focus_" .. elementOrder)
                            playGroupTween("tb_focus_" .. elementOrder, focusBarBg, TweenInfo035, {
                                Size = UDim2.new(0, 0, 1, 0),
                                BackgroundTransparency = 1,
                            })
                            playGroupTween("tb_focus_" .. elementOrder, titleLabel, TweenInfo020, {
                                TextColor3 = palette.TextWhite,
                                TextTransparency = 0,
                            })
                            playGroupTween("tb_focus_" .. elementOrder, charCountLabel, TweenInfo020, {
                                TextTransparency = 0.3,
                            })
                            playGroupTween("tb_focus_" .. elementOrder, inputContainer, TweenInfo020, {
                                BackgroundTransparency = 0.85,
                            })
                        end
                        textBox.Focused:Connect(onFocusEffect)
                        textBox.FocusLost:Connect(function()
                            onBlurEffect()
                            playSound(SOUND_OPEN)
                            callback(textBox.Text)
                        end)
                        textBox:GetPropertyChangedSignal("Text"):Connect(function()
                            local f0 = textBox.Text
                            if maxLength < #f0 then
                                f0 = string.sub(f0, 1, maxLength)
                                textBox.Text = f0
                            end
                            charCountLabel.Text = #f0 .. "/" .. maxLength
                            local f1 = math.clamp(#f0 / maxLength, 0, 1)
                            if f1 > 0.85 then
                                charCountLabel.TextColor3 = Color3.fromRGB(200, 80, 80)
                            elseif f1 > 0.6 then
                                charCountLabel.TextColor3 = palette.AccentBright
                            else
                                charCountLabel.TextColor3 = palette.TextSubtitle
                            end
                        end)
                        inputContainer.InputBegan:Connect(function(f0)
                            if (f0.UserInputType == Enum.UserInputType.MouseMovement) and (not isFocused) then
                                cancelGroupTweens("tbhov_" .. elementOrder)
                                playGroupTween("tbhov_" .. elementOrder, inputContainer, TweenInfo020, {
                                    BackgroundTransparency = 0.65,
                                })
                                playGroupTween("tbhov_" .. elementOrder, boxInnerFrame, TweenInfo020, {
                                    BackgroundTransparency = 0,
                                })
                            end
                        end)
                        inputContainer.InputEnded:Connect(function(f0)
                            if (f0.UserInputType == Enum.UserInputType.MouseMovement) and (not isFocused) then
                                cancelGroupTweens("tbhov_" .. elementOrder)
                                playGroupTween("tbhov_" .. elementOrder, inputContainer, TweenInfo020, {
                                    BackgroundTransparency = 0.85,
                                })
                                playGroupTween("tbhov_" .. elementOrder, boxInnerFrame, TweenInfo020, {
                                    BackgroundTransparency = 0.3,
                                })
                            end
                        end)
                        local inputApi = {
                            Get = function(f0)
                                return textBox.Text
                            end,
                            Set = function(f0, f1)
                                local f2 = string.sub(tostring(f1), 1, maxLength)
                                textBox.Text = f2
                                charCountLabel.Text = #f2 .. "/" .. maxLength
                                callback(f2)
                            end,
                            GetFrame = function(f0)
                                return inputContainer
                            end,
                            SetTitle = function(f0, f1)
                                titleLabel.Text = f1
                            end,
                            SetPlaceholder = function(f0, f1)
                                textBox.PlaceholderText = f1
                            end,
                        }
                        registerSearchItem(inputTitle, "", inputContainer)
                        return inputApi
                    end
                    sectionApi.AddTextbox = function(self, textboxOpts)
                        return self:AddInput(textboxOpts)
                    end
                    sectionApi.AddParagraph = function(self, paragraphOpts)
                        paragraphOpts = paragraphOpts or {}
                        local paragraphTitle = paragraphOpts.Title or "Info"
                        local paragraphContent = ((paragraphOpts.Content or paragraphOpts.Description) or paragraphOpts.Desc) or ""
                        elementOrder = elementOrder + 1
                        local paragraphFrame = Instance.new("Frame")
                        paragraphFrame.BackgroundColor3 = palette.Background
                        paragraphFrame.BackgroundTransparency = 0.85
                        paragraphFrame.Size = UDim2.new(1, 0, 0, 0)
                        paragraphFrame.AutomaticSize = Enum.AutomaticSize.Y
                        paragraphFrame.LayoutOrder = elementOrder
                        paragraphFrame.ZIndex = 3
                        paragraphFrame.Parent = tabPageScroll
                        addPadding(paragraphFrame, 10, 12, 10, 12)
                        applyHoverGlow(paragraphFrame, "para_" .. paragraphTitle .. elementOrder)
                        bindThemeProp(paragraphFrame, "BackgroundColor3", "Background")
                        local hoverGroupKey = "parahov_" .. paragraphTitle .. elementOrder
                        paragraphFrame.InputBegan:Connect(function(f0)
                            if f0.UserInputType == Enum.UserInputType.MouseMovement then
                                cancelGroupTweens(hoverGroupKey)
                                playGroupTween(hoverGroupKey, paragraphFrame, TweenInfo020, {
                                    BackgroundTransparency = 0.5,
                                })
                            end
                        end)
                        paragraphFrame.InputEnded:Connect(function(f0)
                            if f0.UserInputType == Enum.UserInputType.MouseMovement then
                                cancelGroupTweens(hoverGroupKey)
                                playGroupTween(hoverGroupKey, paragraphFrame, TweenInfo020, {
                                    BackgroundTransparency = 0.85,
                                })
                            end
                        end)
                        local paragraphLayout = Instance.new("UIListLayout")
                        paragraphLayout.FillDirection = Enum.FillDirection.Vertical
                        paragraphLayout.Padding = UDim.new(0, 4)
                        paragraphLayout.SortOrder = Enum.SortOrder.LayoutOrder
                        paragraphLayout.Parent = paragraphFrame
                        local textContainer = Instance.new("Frame")
                        textContainer.BackgroundTransparency = 1
                        textContainer.Size = UDim2.new(1, 0, 0, 24)
                        textContainer.LayoutOrder = 1
                        textContainer.ZIndex = 4
                        textContainer.Parent = paragraphFrame
                        local paragraphIcon = Lucide.Resolve(paragraphOpts.Icon, "")
                        if paragraphIcon ~= "" then
                            local e8 = Instance.new("ImageLabel")
                            e8.BackgroundTransparency = 1
                            e8.Size = UDim2.new(0, 22, 0, 22)
                            e8.Position = UDim2.new(0, 0, 0, 1)
                            e8.ScaleType = Enum.ScaleType.Fit
                            e8.Image = paragraphIcon
                            e8.ImageColor3 = palette.Accent
                            e8.ZIndex = 5
                            e8.Parent = textContainer
                            onThemeChange(function()
                                e8.ImageColor3 = palette.Accent
                            end)
                        end
                        local titleLabel = Instance.new("TextLabel")
                        titleLabel.BackgroundTransparency = 1
                        titleLabel.Size = UDim2.new(1, ((paragraphIcon ~= "") and -30) or 0, 1, 0)
                        titleLabel.Position = UDim2.new(0, ((paragraphIcon ~= "") and 28) or 0, 0, 0)
                        titleLabel.FontFace = FontBold
                        titleLabel.TextSize = 13
                        titleLabel.TextColor3 = palette.TextWhite
                        titleLabel.TextXAlignment = Enum.TextXAlignment.Left
                        titleLabel.Text = paragraphTitle
                        titleLabel.ZIndex = 5
                        titleLabel.Parent = textContainer
                        bindThemeProp(titleLabel, "TextColor3", "TextWhite")
                        local contentLabel = Instance.new("TextLabel")
                        contentLabel.BackgroundTransparency = 1
                        contentLabel.Size = UDim2.new(1, 0, 0, 0)
                        contentLabel.AutomaticSize = Enum.AutomaticSize.Y
                        contentLabel.FontFace = FontMedium
                        contentLabel.TextSize = 12
                        contentLabel.TextColor3 = palette.TextSubtitle
                        contentLabel.TextXAlignment = Enum.TextXAlignment.Left
                        contentLabel.TextWrapped = true
                        contentLabel.Text = paragraphContent
                        contentLabel.LayoutOrder = 2
                        contentLabel.ZIndex = 5
                        contentLabel.RichText = true
                        contentLabel.Parent = paragraphFrame
                        bindThemeProp(contentLabel, "TextColor3", "TextSubtitle")
                        local paragraphApi = {
                            SetTitle = function(f0, f1)
                                titleLabel.Text = f1
                            end,
                            SetContent = function(f0, f1)
                                contentLabel.Text = f1
                            end,
                            SetDescription = function(f0, f1)
                                contentLabel.Text = f1
                            end,
                            SetDesc = function(f0, f1)
                                contentLabel.Text = f1
                            end,
                            GetDescriptionLabel = function(f0)
                                return contentLabel
                            end,
                            GetFrame = function(f0)
                                return paragraphFrame
                            end,
                        }
                        registerSearchItem(paragraphTitle, paragraphContent, paragraphFrame)
                        return paragraphApi
                    end
                    sectionApi.AddSeperator = function(self, separatorText)
                        elementOrder = elementOrder + 1
                        local hasTitle = separatorText and (separatorText ~= "")
                        local separatorFrame = Instance.new("Frame")
                        separatorFrame.BackgroundTransparency = 1
                        separatorFrame.Size = UDim2.new(1, 0, 0, (hasTitle and 30) or 16)
                        separatorFrame.LayoutOrder = elementOrder
                        separatorFrame.ZIndex = 3
                        separatorFrame.Parent = tabPageScroll
                        if hasTitle then
                            local e4 = Instance.new("TextLabel")
                            e4.BackgroundTransparency = 1
                            e4.Size = UDim2.new(1, 0, 0, 18)
                            e4.Position = UDim2.new(0, 0, 0, 0)
                            e4.FontFace = FontBold
                            e4.TextSize = 13
                            e4.TextColor3 = Color3.new(1, 1, 1)
                            e4.TextTransparency = 0
                            e4.TextXAlignment = Enum.TextXAlignment.Center
                            e4.Text = separatorText
                            e4.ZIndex = 6
                            e4.Parent = separatorFrame
                        end
                        local lineYPos = (hasTitle and UDim2.new(0, 0, 1, -3)) or UDim2.new(0, 0, 0.5, -1)
                        local leftLine = Instance.new("Frame")
                        leftLine.BackgroundColor3 = palette.Accent
                        leftLine.BackgroundTransparency = 0
                        leftLine.Size = UDim2.new(1, 0, 0, 1)
                        leftLine.Position = lineYPos
                        leftLine.BorderSizePixel = 0
                        leftLine.ZIndex = 5
                        leftLine.Parent = separatorFrame
                        local leftGradient = Instance.new("UIGradient")
                        leftGradient.Transparency = NumberSequence.new({
                            NumberSequenceKeypoint.new(0, 1),
                            NumberSequenceKeypoint.new(0.08, 0),
                            NumberSequenceKeypoint.new(0.92, 0),
                            NumberSequenceKeypoint.new(1, 1),
                        })
                        leftGradient.Rotation = 0
                        leftGradient.Parent = leftLine
                        local rightLine = Instance.new("Frame")
                        rightLine.BackgroundColor3 = palette.Accent
                        rightLine.BackgroundTransparency = 0.55
                        rightLine.Size = UDim2.new(1, 0, 0, 5)
                        rightLine.AnchorPoint = Vector2.new(0, 0.5)
                        rightLine.Position = UDim2.new(0, 0, 0.5, 0)
                        rightLine.BorderSizePixel = 0
                        rightLine.ZIndex = 4
                        rightLine.Parent = leftLine
                        local rightGradient = Instance.new("UIGradient")
                        rightGradient.Transparency = NumberSequence.new({
                            NumberSequenceKeypoint.new(0, 1),
                            NumberSequenceKeypoint.new(0.12, 0.5),
                            NumberSequenceKeypoint.new(0.5, 0.3),
                            NumberSequenceKeypoint.new(0.88, 0.5),
                            NumberSequenceKeypoint.new(1, 1),
                        })
                        rightGradient.Rotation = 0
                        rightGradient.Parent = rightLine
                        local centerLine = Instance.new("Frame")
                        centerLine.BackgroundColor3 = palette.AccentBright
                        centerLine.BackgroundTransparency = 0.3
                        centerLine.Size = UDim2.new(0.4, 0, 0, 3)
                        centerLine.AnchorPoint = Vector2.new(0.5, 0.5)
                        centerLine.Position = UDim2.new(0.5, 0, 0.5, 0)
                        centerLine.BorderSizePixel = 0
                        centerLine.ZIndex = 6
                        centerLine.Parent = leftLine
                        local centerGradient = Instance.new("UIGradient")
                        centerGradient.Transparency = NumberSequence.new({
                            NumberSequenceKeypoint.new(0, 1),
                            NumberSequenceKeypoint.new(0.3, 0.2),
                            NumberSequenceKeypoint.new(0.5, 0),
                            NumberSequenceKeypoint.new(0.7, 0.2),
                            NumberSequenceKeypoint.new(1, 1),
                        })
                        centerGradient.Rotation = 0
                        centerGradient.Parent = centerLine
                        onThemeChange(function()
                            leftLine.BackgroundColor3 = palette.Accent
                            rightLine.BackgroundColor3 = palette.Accent
                            centerLine.BackgroundColor3 = palette.AccentBright
                        end)
                    end
                    sectionApi.AddDiscord = function(self, discordOpts, inviteUrlArg)
                        local serverTitle = discordOpts or "Discord Server"
                        local inviteLink = inviteUrlArg or ""
                        local serverIcon = ""
                        local bannerImage = ""
                        local serverDesc = ""
                        local joinBtnText = "Join Server"
                        if type(discordOpts) == "table" then
                            serverTitle = (discordOpts.Title or discordOpts.Name) or "Discord Server"
                            inviteLink = discordOpts.Link or ""
                            serverIcon = discordOpts.Icon or ""
                            bannerImage = discordOpts.Banner or ""
                            serverDesc = discordOpts.Description or ""
                            joinBtnText = discordOpts.Button or "Join Server"
                        end
                        elementOrder = elementOrder + 1
                        local bannerHeight = 80
                        local avatarSize = 48
                        local avatarRadius = avatarSize / 2
                        local inviteCode = (inviteLink:match("discord%.gg/([^%?#/]+)") or inviteLink:match("discord%.com/invite/([^%?#/]+)")) or inviteLink
                        local hoverGroupKey = "dinv_" .. elementOrder
                        local cardFrame = Instance.new("Frame")
                        cardFrame.BackgroundColor3 = palette.Background
                        cardFrame.BackgroundTransparency = 0.85
                        cardFrame.Size = UDim2.new(1, 0, 0, 0)
                        cardFrame.AutomaticSize = Enum.AutomaticSize.Y
                        cardFrame.LayoutOrder = elementOrder
                        cardFrame.ZIndex = 3
                        cardFrame.ClipsDescendants = false
                        cardFrame.Parent = tabPageScroll
                        addCorner(cardFrame, ITEM_SPACING)
                        local cardStroke = addStroke(cardFrame, palette.Border, 1, 0.5)
                        bindThemeProp(cardFrame, "BackgroundColor3", "Background")
                        bindThemeProp(cardStroke, "Color", "Border")
                        local cardLayout = Instance.new("UIListLayout")
                        cardLayout.FillDirection = Enum.FillDirection.Vertical
                        cardLayout.Padding = UDim.new(0, 0)
                        cardLayout.SortOrder = Enum.SortOrder.LayoutOrder
                        cardLayout.Parent = cardFrame
                        local bannerContainer = Instance.new("Frame")
                        bannerContainer.BackgroundTransparency = 1
                        bannerContainer.Size = UDim2.new(1, 0, 0, bannerHeight)
                        bannerContainer.ClipsDescendants = false
                        bannerContainer.LayoutOrder = 1
                        bannerContainer.ZIndex = 4
                        bannerContainer.Parent = cardFrame
                        local bodyFrame = Instance.new("Frame")
                        bodyFrame.BackgroundColor3 = Color3.fromRGB(28, 28, 32)
                        bodyFrame.Size = UDim2.new(1, 0, 0, bannerHeight + ITEM_SPACING)
                        bodyFrame.ClipsDescendants = true
                        bodyFrame.ZIndex = 4
                        bodyFrame.Parent = bannerContainer
                        addCorner(bodyFrame, ITEM_SPACING)
                        if bannerImage ~= "" then
                            local e19 = Instance.new("ImageLabel")
                            e19.BackgroundTransparency = 1
                            e19.Size = UDim2.new(1, 0, 1, 0)
                            e19.Image = bannerImage
                            e19.ScaleType = Enum.ScaleType.Crop
                            e19.ZIndex = 5
                            e19.Parent = bodyFrame
                        end
                        local avatarOuter = Instance.new("Frame")
                        avatarOuter.BackgroundColor3 = palette.Accent
                        avatarOuter.BackgroundTransparency = 0.45
                        avatarOuter.Size = UDim2.new(1, 0, 0, 2)
                        avatarOuter.Position = UDim2.new(0, 0, 1, -2)
                        avatarOuter.BorderSizePixel = 0
                        avatarOuter.ZIndex = 6
                        avatarOuter.Parent = bodyFrame
                        onThemeChange(function()
                            avatarOuter.BackgroundColor3 = palette.Accent
                        end)
                        local avatarInner = Instance.new("Frame")
                        avatarInner.BackgroundColor3 = Color3.fromRGB(36, 36, 40)
                        avatarInner.Size = UDim2.new(0, avatarSize, 0, avatarSize)
                        avatarInner.Position = UDim2.new(0, 14, 0, bannerHeight - avatarRadius)
                        avatarInner.ZIndex = 8
                        avatarInner.Parent = bannerContainer
                        addCorner(avatarInner, 10)
                        addStroke(avatarInner, palette.Border, 1.5, 0.3)
                        if serverIcon ~= "" then
                            local e21 = Instance.new("ImageLabel")
                            e21.BackgroundTransparency = 1
                            e21.Size = UDim2.new(1, 0, 1, 0)
                            e21.Image = serverIcon
                            e21.ScaleType = Enum.ScaleType.Crop
                            e21.ZIndex = 9
                            e21.Parent = avatarInner
                            addCorner(e21, 10)
                        end
                        local infoContainer = Instance.new("Frame")
                        infoContainer.BackgroundTransparency = 1
                        infoContainer.Size = UDim2.new(1, 0, 0, 0)
                        infoContainer.AutomaticSize = Enum.AutomaticSize.Y
                        infoContainer.LayoutOrder = 2
                        infoContainer.ZIndex = 3
                        infoContainer.Parent = cardFrame
                        addPadding(infoContainer, avatarRadius + 8, 12, 12, 12)
                        local infoLayout = Instance.new("UIListLayout")
                        infoLayout.FillDirection = Enum.FillDirection.Vertical
                        infoLayout.Padding = UDim.new(0, 4)
                        infoLayout.SortOrder = Enum.SortOrder.LayoutOrder
                        infoLayout.Parent = infoContainer
                        local serverNameLabel = Instance.new("TextLabel")
                        serverNameLabel.BackgroundTransparency = 1
                        serverNameLabel.Size = UDim2.new(1, 0, 0, 15)
                        serverNameLabel.LayoutOrder = 1
                        serverNameLabel.ZIndex = 5
                        serverNameLabel.FontFace = FontBold
                        serverNameLabel.TextSize = 13
                        serverNameLabel.TextColor3 = palette.TextWhite
                        serverNameLabel.TextXAlignment = Enum.TextXAlignment.Left
                        serverNameLabel.TextTruncate = Enum.TextTruncate.AtEnd
                        serverNameLabel.Text = serverTitle
                        serverNameLabel.Parent = infoContainer
                        bindThemeProp(serverNameLabel, "TextColor3", "TextWhite")
                        if serverDesc ~= "" then
                            local e24 = Instance.new("TextLabel")
                            e24.BackgroundTransparency = 1
                            e24.Size = UDim2.new(1, 0, 0, 0)
                            e24.AutomaticSize = Enum.AutomaticSize.Y
                            e24.LayoutOrder = 2
                            e24.ZIndex = 5
                            e24.FontFace = FontMedium
                            e24.TextSize = 11
                            e24.TextColor3 = palette.TextSubtitle
                            e24.TextXAlignment = Enum.TextXAlignment.Left
                            e24.TextWrapped = true
                            e24.Text = serverDesc
                            e24.Parent = infoContainer
                            bindThemeProp(e24, "TextColor3", "TextSubtitle")
                        end
                        local statsRow = Instance.new("Frame")
                        statsRow.BackgroundTransparency = 1
                        statsRow.Size = UDim2.new(1, 0, 0, 14)
                        statsRow.LayoutOrder = 3
                        statsRow.ZIndex = 5
                        statsRow.Parent = infoContainer
                        local statsLayout = Instance.new("UIListLayout")
                        statsLayout.FillDirection = Enum.FillDirection.Horizontal
                        statsLayout.VerticalAlignment = Enum.VerticalAlignment.Center
                        statsLayout.HorizontalAlignment = Enum.HorizontalAlignment.Left
                        statsLayout.Padding = UDim.new(0, 10)
                        statsLayout.SortOrder = Enum.SortOrder.LayoutOrder
                        statsLayout.Parent = statsRow
                        local createStatBadge = function(f0, f1, f2)
                            local f3 = Instance.new("Frame")
                            f3.BackgroundTransparency = 1
                            f3.Size = UDim2.new(0, 0, 1, 0)
                            f3.AutomaticSize = Enum.AutomaticSize.X
                            f3.LayoutOrder = f1
                            f3.ZIndex = 6
                            f3.Parent = statsRow
                            local f4 = Instance.new("UIListLayout")
                            f4.FillDirection = Enum.FillDirection.Horizontal
                            f4.VerticalAlignment = Enum.VerticalAlignment.Center
                            f4.Padding = UDim.new(0, 4)
                            f4.SortOrder = Enum.SortOrder.LayoutOrder
                            f4.Parent = f3
                            local f5 = Instance.new("Frame")
                            f5.BackgroundColor3 = f0
                            f5.BackgroundTransparency = 0
                            f5.Size = UDim2.new(0, 7, 0, 7)
                            f5.LayoutOrder = 1
                            f5.ZIndex = 7
                            f5.Parent = f3
                            addCorner(f5, 4)
                            if f2 then
                                onThemeChange(function()
                                    f5.BackgroundColor3 = palette.Accent
                                end)
                            end
                            local f6 = Instance.new("TextLabel")
                            f6.BackgroundTransparency = 1
                            f6.Size = UDim2.new(0, 0, 1, 0)
                            f6.AutomaticSize = Enum.AutomaticSize.X
                            f6.FontFace = FontBold
                            f6.TextSize = 10
                            f6.TextColor3 = palette.TextSubtitle
                            f6.TextTransparency = 0.2
                            f6.TextXAlignment = Enum.TextXAlignment.Left
                            f6.Text = "..."
                            f6.LayoutOrder = 2
                            f6.ZIndex = 7
                            f6.Parent = f3
                            bindThemeProp(f6, "TextColor3", "TextSubtitle")
                            return f6
                        end
                        local onlineStatLabel = createStatBadge(palette.Accent, 1, true)
                        local membersStatLabel = createStatBadge(Color3.fromRGB(120, 120, 120), 2, false)
                        local joinBtnContainer = Instance.new("Frame")
                        joinBtnContainer.BackgroundColor3 = palette.Border
                        joinBtnContainer.BackgroundTransparency = 0.6
                        joinBtnContainer.Size = UDim2.new(1, 0, 0, 1)
                        joinBtnContainer.BorderSizePixel = 0
                        joinBtnContainer.LayoutOrder = 4
                        joinBtnContainer.ZIndex = 5
                        joinBtnContainer.Parent = infoContainer
                        bindThemeProp(joinBtnContainer, "BackgroundColor3", "Border")
                        local joinBtnFrame = Instance.new("Frame")
                        joinBtnFrame.BackgroundColor3 = palette.Background
                        joinBtnFrame.BackgroundTransparency = 0.55
                        joinBtnFrame.Size = UDim2.new(1, 0, 0, 32)
                        joinBtnFrame.LayoutOrder = 5
                        joinBtnFrame.ZIndex = 5
                        joinBtnFrame.Parent = infoContainer
                        addCorner(joinBtnFrame, 6)
                        bindThemeProp(joinBtnFrame, "BackgroundColor3", "Background")
                        local joinBtnStroke = addStroke(joinBtnFrame, palette.Accent, 1.5, 1)
                        onThemeChange(function()
                            joinBtnStroke.Color = palette.Accent
                        end)
                        local joinButton = Instance.new("TextButton")
                        joinButton.BackgroundTransparency = 1
                        joinButton.Size = UDim2.new(1, 0, 1, 0)
                        joinButton.Text = joinBtnText
                        joinButton.FontFace = FontBold
                        joinButton.TextSize = 12
                        joinButton.TextColor3 = Color3.fromRGB(255, 255, 255)
                        joinButton.TextXAlignment = Enum.TextXAlignment.Center
                        joinButton.TextYAlignment = Enum.TextYAlignment.Center
                        joinButton.AutoButtonColor = false
                        joinButton.ZIndex = 6
                        joinButton.Parent = joinBtnFrame
                        joinButton.MouseEnter:Connect(function()
                            cancelGroupTweens(hoverGroupKey .. "_jh")
                            playGroupTween(hoverGroupKey .. "_jh", joinBtnFrame, TweenInfo020, {
                                BackgroundTransparency = 0,
                            })
                            playGroupTween(hoverGroupKey .. "_jh", joinBtnStroke, TweenInfo020, {
                                Transparency = 0,
                            })
                        end)
                        joinButton.MouseLeave:Connect(function()
                            cancelGroupTweens(hoverGroupKey .. "_jh")
                            playGroupTween(hoverGroupKey .. "_jh", joinBtnFrame, TweenInfo020, {
                                BackgroundTransparency = 0.55,
                            })
                            playGroupTween(hoverGroupKey .. "_jh", joinBtnStroke, TweenInfo020, {
                                Transparency = 1,
                            })
                        end)
                        joinButton.MouseButton1Click:Connect(function()
                            if inviteLink == "" then
                                return
                            end
                            playSound(SOUND_OPEN)
                            pcall(function()
                                setclipboard(inviteLink)
                            end)
                            pcall(function()
                                game:GetService("GuiService"):SetClipboard(inviteLink)
                            end)
                            if showNotification then
                                showNotification({
                                    Title = "Copied!",
                                    Text = "Discord link copied to clipboard.",
                                    Duration = 2.5,
                                })
                            end
                        end)
                        task.spawn(function()
                            local f0 = function(g0)
                                g0 = tonumber(g0)
                                if not g0 then
                                    return "N/A"
                                end
                                if g0 >= 1000000 then
                                    return string.format("%.1fM", g0 / 1000000)
                                end
                                if g0 >= 1000 then
                                    return string.format("%.1fk", g0 / 1000)
                                end
                                return tostring(g0)
                            end
                            local f1 = nil
                            if syn and syn.request then
                                f1 = syn.request
                            elseif http and http.request then
                                f1 = http.request
                            else
                                local f2, f3 = pcall(function()
                                    return request
                                end)
                                if f2 and (type(f3) == "function") then
                                    f1 = f3
                                end
                            end
                            while ((onlineStatLabel and onlineStatLabel.Parent) and membersStatLabel) and membersStatLabel.Parent do
                                if ((inviteCode ~= "") and (inviteLink ~= "")) and f1 then
                                    local f2, f3 = pcall(function()
                                        return f1({
                                            Url = "https://discord.com/api/v9/invites/" .. inviteCode .. "?with_counts=true",
                                            Method = "GET",
                                        })
                                    end)
                                    if (f2 and f3) and (f3.StatusCode == 200) then
                                        local f4, f5 = pcall(function()
                                            return game:GetService("HttpService"):JSONDecode(f3.Body)
                                        end)
                                        if f4 and f5 then
                                            if onlineStatLabel and onlineStatLabel.Parent then
                                                onlineStatLabel.Text = f0(f5.approximate_presence_count or 0) .. " Online"
                                            end
                                            if membersStatLabel and membersStatLabel.Parent then
                                                membersStatLabel.Text = f0(f5.approximate_member_count or 0) .. " Members"
                                            end
                                        end
                                    end
                                end
                                task.wait(30)
                            end
                        end)
                        registerSearchItem(serverTitle, "", cardFrame)
                    end
                    sectionApi.AddDropdownWithHoldTime = function(self, holdDropdownOpts)
                        holdDropdownOpts = holdDropdownOpts or {}
                        local dropdownTitle = holdDropdownOpts.Title or "Skills"
                        local optionList = (holdDropdownOpts.Options or holdDropdownOpts.Values) or {}
                        local defaultSelection = holdDropdownOpts.Default or {}
                        if type(defaultSelection) ~= "table" then
                            defaultSelection = {
                                defaultSelection,
                            }
                        end
                        local callback = holdDropdownOpts.Callback or function() end
                        local holdTimeCallback = holdDropdownOpts.HoldTimeCallback or function() end
                        local defaultHoldTime = holdDropdownOpts.DefaultHoldTime or 0.5
                        elementOrder = elementOrder + 1
                        local selectedMap = {}
                        local holdTimeMap = {}
                        for e13, e14 in ipairs(defaultSelection) do
                            selectedMap[tostring(e14)] = true
                        end
                        for e13, e14 in ipairs(optionList) do
                            holdTimeMap[tostring(e14)] = defaultHoldTime
                        end
                        local isOpen = false
                        local dropdownContainer = Instance.new("Frame")
                        dropdownContainer.BackgroundTransparency = 1
                        dropdownContainer.Size = UDim2.new(1, 0, 0, 0)
                        dropdownContainer.AutomaticSize = Enum.AutomaticSize.Y
                        dropdownContainer.LayoutOrder = elementOrder
                        dropdownContainer.ZIndex = 3
                        dropdownContainer.Parent = tabPageScroll
                        local dropdownLayout = Instance.new("UIListLayout")
                        dropdownLayout.FillDirection = Enum.FillDirection.Vertical
                        dropdownLayout.Padding = UDim.new(0, 4)
                        dropdownLayout.SortOrder = Enum.SortOrder.LayoutOrder
                        dropdownLayout.Parent = dropdownContainer
                        local headerFrame = Instance.new("Frame")
                        headerFrame.BackgroundColor3 = palette.Background
                        headerFrame.BackgroundTransparency = 0.85
                        headerFrame.Size = UDim2.new(1, 0, 0, 40)
                        headerFrame.LayoutOrder = 1
                        headerFrame.ZIndex = 4
                        headerFrame.Parent = dropdownContainer
                        addPadding(headerFrame, 6, 12, 6, 12)
                        applyHoverGlow(headerFrame, "ddht_" .. dropdownTitle .. elementOrder)
                        bindThemeProp(headerFrame, "BackgroundColor3", "Background")
                        local titleRow = Instance.new("Frame")
                        titleRow.BackgroundTransparency = 1
                        titleRow.Size = UDim2.new(1, 0, 1, 0)
                        titleRow.ZIndex = 5
                        titleRow.Parent = headerFrame
                        local titleLabel = Instance.new("TextLabel")
                        titleLabel.BackgroundTransparency = 1
                        titleLabel.Size = UDim2.new(1, -22, 0, 16)
                        titleLabel.Position = UDim2.new(0, 0, 0, 0)
                        titleLabel.FontFace = FontBold
                        titleLabel.TextSize = 13
                        titleLabel.TextColor3 = palette.TextWhite
                        titleLabel.TextXAlignment = Enum.TextXAlignment.Left
                        titleLabel.Text = dropdownTitle
                        titleLabel.ZIndex = 6
                        titleLabel.Parent = titleRow
                        bindThemeProp(titleLabel, "TextColor3", "TextWhite")
                        local getSelectedSummary = function()
                            local f0 = {}
                            for f4, f5 in ipairs(optionList) do
                                local f6 = tostring(f5)
                                if selectedMap[f6] then
                                    table.insert(f0, f6 .. "(" .. tostring(holdTimeMap[f6]) .. "s)")
                                end
                            end
                            return ((#f0 > 0) and table.concat(f0, ", ")) or "None"
                        end
                        local selectedSummaryLabel = Instance.new("TextLabel")
                        selectedSummaryLabel.BackgroundTransparency = 1
                        selectedSummaryLabel.Size = UDim2.new(1, -22, 0, 12)
                        selectedSummaryLabel.Position = UDim2.new(0, 0, 0, 16)
                        selectedSummaryLabel.FontFace = FontMedium
                        selectedSummaryLabel.TextSize = 10
                        selectedSummaryLabel.TextColor3 = palette.TextSubtitle
                        selectedSummaryLabel.TextXAlignment = Enum.TextXAlignment.Left
                        selectedSummaryLabel.Text = getSelectedSummary()
                        selectedSummaryLabel.ZIndex = 6
                        selectedSummaryLabel.Parent = titleRow
                        bindThemeProp(selectedSummaryLabel, "TextColor3", "TextSubtitle")
                        local arrowIcon = Instance.new("ImageLabel")
                        arrowIcon.BackgroundTransparency = 1
                        arrowIcon.Size = UDim2.new(0, 14, 0, 14)
                        arrowIcon.AnchorPoint = Vector2.new(1, 0.5)
                        arrowIcon.Position = UDim2.new(1, 0, 0.5, 0)
                        arrowIcon.Image = "rbxassetid://10709790948"
                        arrowIcon.Rotation = 0
                        arrowIcon.ImageColor3 = palette.TextSubtitle
                        arrowIcon.ZIndex = 6
                        arrowIcon.Parent = titleRow
                        bindThemeProp(arrowIcon, "ImageColor3", "TextSubtitle")
                        local drawerClipFrame = Instance.new("Frame")
                        drawerClipFrame.BackgroundTransparency = 1
                        drawerClipFrame.Size = UDim2.new(1, 0, 0, 0)
                        drawerClipFrame.ClipsDescendants = true
                        drawerClipFrame.LayoutOrder = 2
                        drawerClipFrame.ZIndex = 20
                        drawerClipFrame.Parent = dropdownContainer
                        local optionsScroll = Instance.new("ScrollingFrame")
                        optionsScroll.BackgroundColor3 = Color3.fromRGB(15, 15, 15)
                        optionsScroll.Size = UDim2.new(1, 0, 1, 0)
                        optionsScroll.CanvasSize = UDim2.new(0, 0, 0, 0)
                        optionsScroll.AutomaticCanvasSize = Enum.AutomaticSize.Y
                        optionsScroll.ScrollBarThickness = 2
                        optionsScroll.ScrollBarImageColor3 = MutedTextColor
                        optionsScroll.ZIndex = 20
                        optionsScroll.Parent = drawerClipFrame
                        optionsScroll.BorderSizePixel = 0
                        addCorner(optionsScroll, 8)
                        local optionsStroke = addStroke(optionsScroll, palette.Border, 1, 0.45)
                        onThemeChange(function()
                            optionsStroke.Color = palette.Border
                        end)
                        local optionsListLayout = Instance.new("UIListLayout")
                        optionsListLayout.FillDirection = Enum.FillDirection.Vertical
                        optionsListLayout.Padding = UDim.new(0, 5)
                        optionsListLayout.SortOrder = Enum.SortOrder.LayoutOrder
                        optionsListLayout.Parent = optionsScroll
                        addPadding(optionsScroll, 5, 5, 5, 5)
                        local optionRows = {}
                        local fireCallback = function()
                            local f0 = {}
                            for f4, f5 in ipairs(optionList) do
                                local f6 = tostring(f5)
                                if selectedMap[f6] then
                                    table.insert(f0, f6)
                                end
                            end
                            callback(f0, holdTimeMap)
                        end
                        local refreshOptionVisuals = function()
                            selectedSummaryLabel.Text = getSelectedSummary()
                            for f3, f4 in ipairs(optionRows) do
                                local f5 = selectedMap[f4._val] == true
                                TweenService:Create(f4._bar, TweenInfo020, {
                                    BackgroundTransparency = (f5 and 0) or 1,
                                }):Play()
                                TweenService:Create(f4._frame, TweenInfo020, {
                                    BackgroundTransparency = (f5 and 0.82) or 1,
                                    BackgroundColor3 = palette.Background,
                                }):Play()
                                TweenService:Create(f4._lbl, TweenInfo020, {
                                    TextColor3 = (f5 and palette.AccentBright) or palette.TextWhite,
                                }):Play()
                            end
                        end
                        for e29, e30 in ipairs(optionList) do
                            local e31 = tostring(e30)
                            local e32 = selectedMap[e31] == true
                            local e33 = Instance.new("Frame")
                            e33.BackgroundColor3 = palette.Background
                            e33.BackgroundTransparency = (e32 and 0.82) or 1
                            e33.Size = UDim2.new(1, 0, 0, 30)
                            e33.LayoutOrder = e29
                            e33.ZIndex = 21
                            e33.Parent = optionsScroll
                            addCorner(e33, 5)
                            bindThemeProp(e33, "BackgroundColor3", "Background")
                            local e34 = Instance.new("Frame")
                            e34.BackgroundColor3 = palette.Accent
                            e34.BackgroundTransparency = (e32 and 0) or 1
                            e34.Size = UDim2.new(0, 2, 1, -8)
                            e34.Position = UDim2.new(0, 1, 0, 4)
                            e34.ZIndex = 22
                            e34.Parent = e33
                            addCorner(e34, 1)
                            onThemeChange(function()
                                e34.BackgroundColor3 = palette.Accent
                            end)
                            local e35 = Instance.new("TextLabel")
                            e35.BackgroundTransparency = 1
                            e35.Size = UDim2.new(0.5, -14, 0, 13)
                            e35.Position = UDim2.new(0, 10, 0, 8)
                            e35.FontFace = FontBold
                            e35.TextSize = 11
                            e35.TextColor3 = (e32 and palette.AccentBright) or palette.TextWhite
                            e35.TextXAlignment = Enum.TextXAlignment.Left
                            e35.Text = e31
                            e35.ZIndex = 22
                            e35.Parent = e33
                            bindThemeProp(e35, "TextColor3", "TextWhite")
                            local e36 = Instance.new("Frame")
                            e36.BackgroundColor3 = Color3.fromRGB(20, 20, 20)
                            e36.BackgroundTransparency = 0.4
                            e36.Size = UDim2.new(0, 70, 0, 22)
                            e36.Position = UDim2.new(1, -76, 0, 4)
                            e36.ZIndex = 22
                            e36.Parent = e33
                            addCorner(e36, 4)
                            local e37 = Instance.new("TextLabel")
                            e37.BackgroundTransparency = 1
                            e37.Size = UDim2.new(0, 30, 1, 0)
                            e37.Position = UDim2.new(0, 4, 0, 0)
                            e37.FontFace = FontMedium
                            e37.TextSize = 9
                            e37.TextColor3 = palette.TextSubtitle
                            e37.Text = "Hold:"
                            e37.ZIndex = 23
                            e37.Parent = e36
                            bindThemeProp(e37, "TextColor3", "TextSubtitle")
                            local e38 = Instance.new("TextBox")
                            e38.BackgroundTransparency = 1
                            e38.Size = UDim2.new(0, 32, 1, 0)
                            e38.Position = UDim2.new(0, 32, 0, 0)
                            e38.FontFace = FontBold
                            e38.TextSize = 11
                            e38.TextColor3 = palette.TextWhite
                            e38.PlaceholderText = "0.5"
                            e38.Text = tostring(defaultHoldTime)
                            e38.ClearTextOnFocus = false
                            e38.ZIndex = 24
                            e38.Parent = e36
                            bindThemeProp(e38, "TextColor3", "TextWhite")
                            local e39 = e31
                            e38.FocusLost:Connect(function()
                                local f0 = tonumber(e38.Text)
                                if (f0 and (f0 >= 0)) and (f0 <= 30) then
                                    holdTimeMap[e39] = f0
                                    holdTimeCallback(e39, f0)
                                    selectedSummaryLabel.Text = getSelectedSummary()
                                    if _G and _G.AutoSaveHook then
                                        _G.AutoSaveHook("NM_HT_" .. dropdownTitle .. "_" .. e39, f0)
                                    end
                                else
                                    e38.Text = tostring(holdTimeMap[e39] or defaultHoldTime)
                                end
                            end)
                            if _G and _G.AutoLoadHook then
                                local e40 = _G.AutoLoadHook("NM_HT_" .. dropdownTitle .. "_" .. e39, nil)
                                if e40 then
                                    holdTimeMap[e39] = e40
                                    e38.Text = tostring(e40)
                                end
                            end
                            local e39_2 = Instance.new("TextButton")
                            e39_2.BackgroundTransparency = 1
                            e39_2.Size = UDim2.new(0.5, 0, 1, 0)
                            e39_2.Text = ""
                            e39_2.ZIndex = 23
                            e39_2.AutoButtonColor = false
                            e39_2.Parent = e33
                            local e40 = e31
                            local e41 = "ddhtopt_" .. e40 .. elementOrder
                            e39_2.MouseEnter:Connect(function()
                                if not selectedMap[e40] then
                                    cancelGroupTweens(e41)
                                    playGroupTween(e41, e33, TweenInfo020, {
                                        BackgroundColor3 = palette.Background,
                                        BackgroundTransparency = 0.88,
                                    })
                                end
                            end)
                            e39_2.MouseLeave:Connect(function()
                                if not selectedMap[e40] then
                                    cancelGroupTweens(e41)
                                    playGroupTween(e41, e33, TweenInfo020, {
                                        BackgroundColor3 = palette.Background,
                                        BackgroundTransparency = 1,
                                    })
                                end
                            end)
                            e39_2.MouseButton1Click:Connect(function()
                                playSound(SOUND_OPEN)
                                selectedMap[e40] = not selectedMap[e40]
                                refreshOptionVisuals()
                                fireCallback()
                            end)
                            table.insert(optionRows, {
                                _frame = e33,
                                _bar = e34,
                                _val = e31,
                                _lbl = e35,
                            })
                        end
                        onThemeChange(function()
                            for f3, f4 in ipairs(optionRows) do
                                f4._bar.BackgroundColor3 = palette.Accent
                                f4._lbl.TextColor3 = (selectedMap[f4._val] and palette.AccentBright) or palette.TextWhite
                            end
                        end)
                        local drawerTargetHeight = math.min(10 + (#optionList * 34), 180)
                        local openDropdown = function()
                            isOpen = true
                            cancelGroupTweens("ddhtmenu_" .. elementOrder)
                            playGroupTween("ddhtmenu_" .. elementOrder, drawerClipFrame, TweenInfo035, {
                                Size = UDim2.new(1, 0, 0, drawerTargetHeight),
                            })
                            playGroupTween("ddhtmenu_" .. elementOrder, headerFrame, TweenInfo020, {
                                BackgroundTransparency = 0.7,
                            })
                            playGroupTween("ddhtmenu_" .. elementOrder, arrowIcon, TweenInfo020, {
                                Rotation = 180,
                            })
                        end
                        local closeDropdown = function()
                            isOpen = false
                            cancelGroupTweens("ddhtmenu_" .. elementOrder)
                            playGroupTween("ddhtmenu_" .. elementOrder, drawerClipFrame, TweenInfo020, {
                                Size = UDim2.new(1, 0, 0, 0),
                            })
                            playGroupTween("ddhtmenu_" .. elementOrder, headerFrame, TweenInfo020, {
                                BackgroundTransparency = 0.85,
                            })
                            playGroupTween("ddhtmenu_" .. elementOrder, arrowIcon, TweenInfo020, {
                                Rotation = 0,
                            })
                        end
                        local hoverGroupKey = "ddhthov_" .. dropdownTitle .. elementOrder
                        headerFrame.InputBegan:Connect(function(f0)
                            if f0.UserInputType == Enum.UserInputType.MouseMovement then
                                cancelGroupTweens(hoverGroupKey)
                                if not isOpen then
                                    playGroupTween(hoverGroupKey, headerFrame, TweenInfo020, {
                                        BackgroundTransparency = 0.5,
                                    })
                                end
                            end
                        end)
                        headerFrame.InputEnded:Connect(function(f0)
                            if f0.UserInputType == Enum.UserInputType.MouseMovement then
                                cancelGroupTweens(hoverGroupKey)
                                if not isOpen then
                                    playGroupTween(hoverGroupKey, headerFrame, TweenInfo020, {
                                        BackgroundTransparency = 0.85,
                                    })
                                end
                            end
                        end)
                        local headerToggleBtn = Instance.new("TextButton")
                        headerToggleBtn.BackgroundTransparency = 1
                        headerToggleBtn.Size = UDim2.new(1, 0, 1, 0)
                        headerToggleBtn.Text = ""
                        headerToggleBtn.ZIndex = 7
                        headerToggleBtn.AutoButtonColor = false
                        headerToggleBtn.Parent = headerFrame
                        headerToggleBtn.MouseButton1Click:Connect(function()
                            if isOpen then
                                closeDropdown()
                            else
                                openDropdown()
                            end
                        end)
                        local holdDropdownApi = {
                            GetSelected = function(f0)
                                local f1 = {}
                                for f5, f6 in ipairs(optionList) do
                                    local f7 = tostring(f6)
                                    if selectedMap[f7] then
                                        table.insert(f1, f7)
                                    end
                                end
                                return f1
                            end,
                            GetHoldTime = function(f0, f1)
                                return holdTimeMap[tostring(f1)] or defaultHoldTime
                            end,
                            GetAll = function(f0)
                                local f1 = {}
                                for f5, f6 in ipairs(optionList) do
                                    local f7 = tostring(f6)
                                    f1[f7] = {
                                        selected = selectedMap[f7] == true,
                                        holdTime = holdTimeMap[f7] or defaultHoldTime,
                                    }
                                end
                                return f1
                            end,
                            Close = function(f0)
                                closeDropdown()
                            end,
                            Open = function(f0)
                                openDropdown()
                            end,
                        }
                        task.defer(function()
                            fireCallback()
                        end)
                        registerSearchItem(dropdownTitle, "", dropdownContainer)
                        return holdDropdownApi
                    end
                    return sectionApi
                end,
            }
        end
        return {
            T = createTab,
            Tab = createTab,
            AddTab = createTab,
            NewTab = createTab,
            CreateTab = createTab,
            GetIcon = function(self, iconName)
                return Lucide.GetIcon(iconName)
            end,
            Notify = function(self, c0)
                c0 = c0 or {}
                if showNotification then
                    showNotification(c0)
                end
            end,
        }
    end)()
end
return VexzHub
