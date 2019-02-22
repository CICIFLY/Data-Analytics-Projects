À

ÀÇÅ
Fuel Economy Guide Database files.

The ZIP'd versions of these files are named ??DATA.ZIP (e.g., 83DATA.ZIP)
for 1978-1983 database files, ??MFGUI.ZIP (e.g., 93MFGUI.ZIP) for
1984-1997 and  ??GUIDE.ZIP for 1998 and later model year database files.

Following are notes about the files included in the ZIP's,
then definitions of abbreviations that are used in the reports, and
then detailed database format information for the four different
formats that are used, depending on model year.

This information is provided by the U.S. Environmental Protection Agency,
Office of Mobile Sources, National Vehicle and Fuel Emissions Laboratory,
2000 Traverwood, Ann Arbor, MI 48105 (734-214-4200).

      ===================================================

Up to the 1985 model year, fuel economy guides were generated
separately for 49-state and California. 

For model year 1983 and earlier model years, files named ??FG.DAT contain models
for 49-state and ??CG.DAT contain those for California.

For model years 1984 and 1985, models for both of the sales areas
are included in the file ??MFGUI.DAT and the sales area of a
particular model is identified in the field named 'STATE CODE'.

For model years 1998 and later, both comma-delimited (??GUIDE6.CSV)
and Excel spreadsheet (??GUIDE6.XLS) format files are included. 
For 2000 and later, additional files ??GD_ALT.CSV and ??GD_ALT.XLS 
are included for alternative fueled vehicles.
 
For model year 1997 and earlier, interior volumes for available body styles (2-dr, 4-dr and
hatchback) or vehicle class name (compact car, mid-size car, etc)
for a model type in the files ??CG.DAT or ??FG.DAT can be retrieved
from ??CARLN.DAT by relating the 5-digit carline code and the 2-
digit class code in the files.


      ===================================================


DEFINITION OF REPORT ABBREVIATIONS
åAn explanation of abbreviations used in the Fuel Economy Guide 
and Test Car List reports published by EPA follows:


Car Line Name and Vehicle ID (Guide and Test Car List)

    These are manufacturer-determined descriptors.

         * Test type 31 data = fuel economy data
         # Test type 32 data = analytical data

Engine Description (Guide and Test Car List)

    (GUZZLER)              -- Gas Guzzler
    (POLICE)               -- Police vehicle
    (MPFI), (MPI*)         -- Multipoint fuel injection
    (SPFI)                 -- Single-point fuel injection
    (FFS)                  -- Feedback fuel system
    (TURBO), (TRBO), (TC*) -- Turbocharger
    (S-CHARGE), (SC*)      -- Supercharger
    (DIESEL), (DSL)        -- Diesel
    (ROTARY)               -- Rotary engine
    (VARIABLE)             -- Variable displacement engine
    (NO-CAT)               -- No catalytic converter
    (OHC)                  -- Overhead camshaft
    (OHV)                  -- Overhead valves
    (16-VALVE)             -- 16-valves
    (305)                  -- 305 cubic inch displacement
    (307)                  -- 307 cubic inch displacement
    (M-ENG)                -- One of two 5.8L Ford truck engines
    (W-ENG)                -- One of two 5.8L Ford truck engines
    (GM-BUICK)             -- Engine produced by GM-Buick Motor Division
    (GM-CHEV)              -- Engine produced by GM-Chevrolet Motor Division
    (GM-OLDS)              -- Engine produced by GM-Oldsmobile Motor Division
    (GM-PONT)              -- Engine produced by GM-Pontiac Motor Division

Any other descriptors not listed here are those submitted by manufacturers to
augment engine information and may not always be self-explanatory.

Transmission Descriptors  (Guide and Test Car List)

    First Character --               OD  (Overdrive Code)
         M -- Manual                      1 -- No gear ratio < 1.0
         A -- Automatic                   2 -- High gear ratio < 1.0
         L -- Lockup/automaticå         S -- Semiautomatic

    Second Character -- Number of forward speeds
         V -- Fully variable gear ratios

    Third Character -- (optional, Guide only)
         C -- Creeper

Drive System (Guide and Test Car List)    FWD -- Front-wheel drive
                                          RWD -- Rear-wheel drive
                                          4WD -- Four-wheel drive




Transmission Description (Guide and Test Car List)

    EMS         -- Engine management system
    SIL         -- Shift indicator light on instrument panel
    CLKUP       -- Computer-controlled continuously variable lockup
    VLKUP       -- Continuously variable, user-selectable lockup
    nLKUP       -- User-selectable lockup with n (2 through 9) lockup ranges
    CMODE       -- Computer controlled multimode transmission
    VMODE       -- User-selectable continuously variable transmission
    nMODE       -- Multimode, user-selectable transmission**
                           n = number of gear ranges (2 through 9)
    DC/FW or FW -- Declutching and freewheeling

** An automatic transmission that has an operator-selectable feature that 
changes
   transmission parameters such as gear ratios or automatic transmission shift
   speed calibrations; e.g.: transmissions with "power" and "economy" modes.

Fuel System (Guide and Test Car List)

    FI   -- Fuel injection
    1    -- 1-barrel carburetor
    2    -- 2-barrel carburetor
    3    -- 3-barrel carburetor
    4    -- 4-barrel carburetor

Fuel Type (Guide)

    P    -- Premium unleaded gasoline
    R    -- Regular unleaded gasolineå    D    -- Diesel fuel
    C    · · Compressed natural gas
    E    · · Ethanol

Control System (Test Car List)

    AIR         -- Air Injection
    EM          -- Engine Modification
    FI          -- Fuel Injection
    THM         -- Thermal Reactor
    CAT         -- Catalyst
    TUR,       -- Turbocharger
    EGR         -- Exhaust Gas Recycle
    NON         -- None
    PMP         -- Air Pump
    PLS,        -- Pulsating Air System
    OXD,      -- Oxidation Catalyst
    RED         -- Reduction Catalyst
    3WY        - Three-way Catalyst
    CLS         -- Closed Loop
    3CL         -- Three-way Catalyst + Closed Loop
    CAI         -- Closed Loop Air Injection
    OTR         -- Other


      ===================================================


Database Formats
----------------

There are different formats for these database files depending on
the model year.  Following are the database formats for:

1998 and later
1985-1997
1984,
1978-1983


   =================================================================

Database formats for 1998 and later Fuel Economy Guide Database files.
The comma-delimited format files are named ??GUIDE6.CSV and the Excel spreadsheet 
format files are named ??GUIDE6.XLSåclass     - vehicle class name
manufacturer  -  manufacturer or division name
carline name   - model name
displ    - displacement in liters
cyl       - number of engine cylinders
trans    - transmission type
drv      - drive axle type:
       F - front wheel drive
       R - rear wheel drive
       4  - 4-wheel or all-wheel drive
cty       - estimated city mpg (miles/gallon)
hwy     - estimated highway mpg (miles/gallon)
cmb     - estimated combined mpg (miles/gallon)
ucty     - unadjusted city mpg
uhwy   -unadjusted highway mpg
ucmb   - unadjusted combined mpg
fl         - fuel type:
      R - regular grade gasoline (octane number of 87)
      P - premium grade gasoline (octane number  of 92 or 93)
      D - diesel fuel
     C - compressed natural gas
     E - ethanol (E85 - 85% ethanol, 15% gas
     El  - electricity 
G         - the model is a gas guzzler if this column has a 'G'
T          - the model is equipped with turbocharger if this column has a 'T'
S          - the model is equipped with supercharger if this column has an 'S'
2pv      - passenger interior volume of  a 2-door version
2lv       - luggage interior volume of a 2-door version
4pv      - passenger interior volume of a 4-door version
4lv       - luggage interior volume of a 4-door version
hpv      - passenger interior volume of a hatchback version
hlv       - luggage interior volume of a hatchback version
fcost    - annual fuel cost based on estimated combined mpg
eng dscr - an engine related descriptor to identify a model from another similar model
trans dscr - a transmission related descriptor to identify a model from another similar model
vpc       © valves per cylinder (for 2000 or later only)
cls         © vehicle class code(1=2©seater, 2=minicompact, etc) (for 2000 or later only)

Passenger/luggage interior volume is shown for available body types only.

Interior volume dimensions are not required for Two Seater passenger cars or any vehicle
classified as truck which includes vans, pickups, special purpose vehicles, minivan and sport
utility vehicles.

         =================================================================åDatabase format for 1985-1997 Fuel Economy Guide Database files.
The ZIP'd versions of these files are named ??MFGUI.ZIP, e.g., 93MFGUI.ZIP.

:
1***********************************                                                                    
*************************
 * ENVIRONMENTAL PROTECTION AGENCY *                                                                    
* DATE RUN:OCT  7, 1987 *
 * MOTOR VEHICLE EMISSIONS LAB     *                                                                     *
TIME RUN:09:50:16     *
 * ANN ARBOR, MICHIGAN             *                                                                     * PAGE
NUMBER:   1      *
 ***********************************                                                                    
*************************
0                                                     DATA FILE DEFINITION
                                                     **********************
                                                     *                    *
                                                     * MFGUI85 - MFGUI93  *
                                                     *                    *
                                                     **********************
0                                                                 FILE DESCRIPTION

******************************************************************************
**************************************************
**
                                                                * Fuel Economy Guide data bases for 1985-1993 model
year

******************************************************************************
**************************************************
**
0 RECORD  FIELD       FIELD     STARTING               #DEC.
    ID    NUMBER       NAME      COLUMN   WIDTH  TYPE  PLACES  COMMENTS
0*****************************************************************************
**************************************************
***
     1       1     ACTIVE YEAR       1       4    I      0     ACTIVE YEAR
     1       2     STATE CODE        5       1    A      0     STATE CODE:  F=49-STATE,
C=CALIFORNIA
     1       3     CARLINE CLSS      6       2    I      0     CARLINE CLASS CODE
     1       4     CARLINE MFR CODE  8       3    I      0     CARLINE MANUFACTURER CODE
     1       5     CARLINE NAME     11      28    A      0     CARLINE NAME
     1       6     DISP CUB IN      39       4    I      0     DISP CUBIC INCHES
     1       7     FUEL SYSTEM      43       2    A      0     FUEL SYSTEM: 'FI' FOR FUEL
INJECTION, 2-DIGIT INTEGER VALUEå                                                                            FOR #OF VENTURIES IF CARBURETOR
SYSTEM.
     1       8     MODEL TRANS      45       6    A      0     TRANSMISSION TYPE
     1       9     NO CYC           51       2    I      0     NUMBER OF ENGINE CYLINDERS
     1      10     DATE   TIME      53      12    A      0     DATE AND TIME RECORD ENTERED -
YYMMDDHHMMSS (YEAR, MONTH, DAY,
                                                                                              HOUR, MINUTE, SECOND)
     1      11     RELEASE DATE     65       6    A      0     RELEASE DATE - YYMMDD (YEAR,
MONTH, DAY)
     1      12     VI MFR CODE      71       3    I      0     VI MANUFACTURER CODE
     1      13     CARLINE CODE     74       5    I      0     CARLINE CODE
     1      14     BASIC ENG ID     79       5    I      0     BASIC ENGINE INDEX
     1      15     CARLINE MFR NAME 84      32    A      0     CARLINE MANUFACTURER
NAME
     1      16     SUPPRESS CODE   116       1    I      0     SUPPRESSION CODE (NO
SUPPRESSED RECORD IF FOR PUBLIC ACCESS)
     1      17     EST CITY MPG    117       3    I      0     ESTIMATED (CITY) MILES PER
GALLON - 90% OF UNADJUSTED VALUE
     1      18     HIGHWAY MPG     122       3    I      0     ESTIMATED (HWY) MILES PER
GALLON - 78% OF UNADJUSTED VALUE
     1      19     COMBINED MPG    127       3    I      0     COMBINED MILES PER GALLON
     1      20     UNADJ CITY MPG  132       3    I      0     UNADJUSTED  CITY MILES PER
GALLON
     1      21     UNADJ HWY MPG   137       3    I      0     UNADJUSTED HIGHWAY MILES
PER GALLON
     1      22     UNADJ COMB MPG  142       3    I      0     UNADJUSTED COMBINED MILES
PER GALLON
     1      23     AVE ANL FUEL    147       6    I      0     "$" in col 147, Annual Fuel Cost starting
col 148 in I5
     1      24     OPT DISP        153       8    A      0     OPTIONAL DISPLACEMENT
     1      26     ENGINE DESC1    161      10    A      0     ENGINE DESCRIPTION 1
     1      27     ENGINE DESC2    171      10    A      0     ENGINE DESCRIPTION 2
     1      28     ENGINE DESC3    181      10    A      0     ENGINE DESCRIPTION 3
     1      29     BODY TYPE 2D    191      10    A      0     BODY TYPE 2 DOOR - IF THE BODY
TYPE APPLIES IT WILL TAKE THE
                                                               FORM '2DR-PPP/LL' WHERE PPP=PASSENGER
INTERIOR VOLUME AND
                                                               LL=LUGGAGE INTERIOR VOLUME.
     1      30     BODY TYPE 4D    201      10    A      0     BODY TYPE 4 DOOR - IF THE BODY
TYPE APPLIES IT WILL TAKE THE
                                                               FORM '4DR-PPP/LL' WHERE PPP=PASSENGER
INTERIOR VOLUME AND
                                                               LL=LUGGAGE INTERIOR VOLUME.
     1      31     BODY TYPE HBK   211      10    A      0     BODY TYPE HBK    - IF THE BODY
TYPE APPLIES IT WILL TAKE THEå                                                               FORM 'HBK-PPP/LL' WHERE PPP=PASSENGER
INTERIOR VOLUME AND
                                                               LL=LUGGAGE INTERIOR VOLUME.
     1      32     PUERTO RICO     221       1    A      0     '*' IF FOR PUERTO RICO SALES
ONLY
     1      33     OVERDRIVE       222       4    A      0     OVERDRIVE:  ' OD ' FOR
OVERDRIVE, 'EOD ' FOR ELECTRICALLY OPERATED
                                                               OVERDRIVE AND 'AEOD' FOR AUTOMATIC
OVERDRIVE
     1      34     DRIVE SYSTEM    226       3    A      0     FWD=FRONT WHEEL DRIVE, 
RWD=REAR,  4WD=4-WHEEL
     1      35     FILLER          229       1    A      0     NOT USED
     1      36     FUEL TYPE       230       1    A      0     R=REGULAR(UNLEADED), 
P=PREMIUM,  D=DIESEL
     1      37     TRANS DESC      231      15    A      0     TRANSMISSION DESCRIPTORS

   =================================================================


Database format for 1984 Fuel Economy Guide Database file.
The ZIP'd versions of this file is named 84MFGUI.ZIP.

:
1***********************************                                                                    
*************************
 * ENVIRONMENTAL PROTECTION AGENCY *                                                                    
* DATE RUN:OCT  7, 1987 *
 * MOTOR VEHICLE EMISSIONS LAB     *                                                                     *
TIME RUN:09:50:16     *
 * ANN ARBOR, MICHIGAN             *                                                                     * PAGE
NUMBER:   1      *
 ***********************************                                                                    
*************************
0                                                     DATA FILE DEFINITION
                                                     **********************
                                                     *                    *
                                                     *      MFGUI84       *
                                                     *                    *
                                                     **********************
0                                                                 FILE DESCRIPTION

******************************************************************************
**************************************************
**
                                                                * Fuel Economy Guide data base for 1984 model yearå******************************************************************************
**************************************************
**
0 RECORD  FIELD       FIELD     STARTING               #DEC.
    ID    NUMBER       NAME      COLUMN   WIDTH  TYPE  PLACES  COMMENTS
0*****************************************************************************
**************************************************
***
     1       1     ACTIVE YEAR       1       4    I      0     ACTIVE YEAR
     1       2     STATE CODE        5       1    A      0     STATE CODE:  F=49-STATE,
C=CALIFORNIA
     1       3     CARLINE CLSS      6       2    I      0     CARLINE CLASS CODE
     1       4     CARLINE MFR       8       3    I      0     CARLINE MANUFACTURER CODE
     1       5     CARLINE NAME     11      28    A      0     CARLINE NAME
     1       6     DISP CUB IN      39       4    I      0     DISP CUBIC INCHES
     1       7     FUEL SYSTEM      43       2    A      0     FUEL SYSTEM: 'FI' FOR FUEL
INJECTION, 2-DIGIT INTEGER VALUE
                                                                            FOR #OF VENTURIES IF CARBURETOR
SYSTEM.
     1       8     MODEL TRANS      45       6    A      0     TRANSMISSION TYPE
     1       9     NO CYC           51       2    I      0     NUMBER OF ENGINE CYLINDERS
     1      10     DATE   TIME      53      12    A      0     DATE AND TIME RECORD ENTERED -
YYMMDDHHMMSS (YEAR, MONTH, DAY,
                                                                                              HOUR, MINUTE, SECOND)
     1      11     RELEASE DATE     65       6    A      0     RELEASE DATE - YYMMDD (YEAR,
MONTH, DAY)
     1      12     VI MFR CODE      71       3    I      0     VI MANUFACTURER CODE
     1      13     FILLER           74       5    H      0     NOT USED
     1      14     BASIC ENG ID     79       5    I      0     BASIC ENGINE INDEX
     1      15     CARLINE MFR NAME 84      32    A      0     CARLINE MANUFACTURER
NAME
     1      16     SUPPRESS CODE   116       1    I      0     SUPPRESSION CODE (NO
SUPPRESSED RECORD IF FOR PUBLIC ACCESS)
     1      17     FILLER          117      15    H      0     NOT USED
     1      18     EST CITY MPG    132       3    I      0     ESTIMATED (CITY) MILES PER
GALLON
     1      19     HIGHWAY MPG     137       3    I      0     HIGHWAY MILES PER GALLON
     1      20     COMBINED MPG    142       3    I      0     COMBINED MILES PER GALLON
     1      21     AVE ANL FUEL    147       6    A      0     "$" in col 147, Annual Fuel Cost starting
col 148, in I5
     1      22     OPT DISP        153       8    A      0     OPTIONAL DISPLACEMENT
     1      23     ENGINE DESC1    161      10    A      0     ENGINE DESCRIPTION 1
     1      24     ENGINE DESC2    171      10    A      0     ENGINE DESCRIPTION 2
     1      25     FILLER          181      10    H      0     NOT USED
     1      26     BODY TYPE 2D    191      10    A      0     BODY TYPE 2 DOOR - IF THE BODYåTYPE APPLIES IT WILL TAKE THE
                                                               FORM '2DR-PPP/LL' WHERE PPP=PASSENGER
INTERIOR VOLUME AND
                                                               LL=LUGGAGE INTERIOR VOLUME.
     1      27     BODY TYPE 4D    201      10    A      0     BODY TYPE 4 DOOR - IF THE BODY
TYPE APPLIES IT WILL TAKE THE
                                                               FORM '4DR-PPP/LL' WHERE PPP=PASSENGER
INTERIOR VOLUME AND
                                                               LL=LUGGAGE INTERIOR VOLUME.
     1      28     BODY TYPE HBK   211      10    A      0     BODY TYPE HBK    - IF THE BODY
TYPE APPLIES IT WILL TAKE THE
                                                               FORM 'HBK-PPP/LL' WHERE PPP=PASSENGER
INTERIOR VOLUME AND
                                                               LL=LUGGAGE INTERIOR VOLUME.
     1      28     PUERTO RICO     221       1    A      0     '*' IF FOR PUERTO RICO SALES
ONLY
     1      29     OVERDRIVE       222       4    A      0     '(OD)' IF ELECTRICALLY OPERATED
OVERDRIVE

   =================================================================


Database format for 1978-1983 Fuel Economy Guide Database files.
The ZIP'd versions of these files are named ??DATA.ZIP, e.g., 83DATA.ZIP.

:
1***********************************                                                                    
*************************
 * ENVIRONMENTAL PROTECTION AGENCY *                                                                    
* DATE RUN:OCT  7, 1987 *
 * MOTOR VEHICLE EMISSIONS LAB     *                                                                     *
TIME RUN:09:50:16     *
 * ANN ARBOR, MICHIGAN             *                                                                     * PAGE
NUMBER:   1      *
 ***********************************                                                                    
*************************
0                                                     DATA FILE DEFINITION
                                                     ************************
                                                     *                      *
                                                     *  78CG.DAT, 78FG.DAT  *
                                                     *        ...           *
                                                     *  83CG.DAT, 83FG.DAT  *
                                                     ************************
0                                                                 FILE DESCRIPTION
å******************************************************************************
**************************************************
**
                                                                * FILE PURPOSE:  FUEL ECONOMY GUIDE DATA
BASES for 1978 TO 1983
                                                                * RESTRICTED INFORMATION IS THE
                                                                * SALES WHICH ARE NEVER MADE PUBLIC
INFORMATION.
 COMMENT  #1  -  MODEL  LEVEL  TRANSMISSION  CODE  IS  DETERMINED  BY 
MODTRS(FIELD#  15)  AND MODTRN(FIELD #21): MODEL
LEVEL
 TRANSMISSION IS M3/M4C IF MODTRS=M3 &MODTRN=C, M4C IF MODTRS=C4 &
MODTRN=C, M4X2 IF MODTRS=D4 AND IT IS THE SAME 
AS  MODTRS
 FOR  OTHER CASES EXCEPT THAT IF THE O-D-CODE(FIELD #17) IS 3, (OD) IS
APPENDED TO MODTRS.

******************************************************************************
**************************************************
**
0 RECORD  FIELD       FIELD     STARTING               #DEC.
    ID    NUMBER       NAME      COLUMN   WIDTH  TYPE  PLACES  COMMENTS
0*****************************************************************************
**************************************************
***
     1       1     SUPPRESS          1       1    I      0     NUMERIC CODE FOR REASON FOR
SUPPRESSION: NO SUPPRESSED RECORD
                                                               IF FOR PUBLIC ACCESS
     1       2     ALT-LOW           2       1    I      0     LOW ALTITUDE APPLICATION: 0 OR
BLANK- NO,  1 - YES
     1       3     ALT-HIGH          3       1    I      0     HIGH ALTITUDE APPLICATION: 0 OR
BLANK - NO,  1 - YES
     1       4     ALT-BOTH          4       1    I      0     LOW & HIGH ALTITUDE APPLICATION: 
0 OR BLANK - NO,  1 - YES
     1       6     BAS-ENG-INDX      6       5    I      0     5 DIGIT NUMBER IDENTIFYING A
GROUP INFO FOR A BASIC ENGINE
     1       7     CARLINE-CODE     11       5    I      0     CARLINE CODE--5 DIGIT CODE
ASSIGNED TO A CARLINE. THE FIRST
                                                               3 DIGITS REPRESENT A CARLINE
MANUFACTURER (PARTICULAR MANUFACTURER
                                                               OR DIVISION WITHIN A CORPORATE ENTITY).
AND THE LAST TWO DIGITS
                                                               REPRESENT AN ARBITRARY NUMBER ASSIGNED
TO A CARLINE.  INFORMATION
                                                               RELATING TO A CARLINE CODE CAN BEåOBTAINED FROM CARLINE DATA FILE.
     1       8     FILLER           16       3    H      0     NOT USED
     1       9     CARLINE-CLAS     19       2    I      0     CARLINE CLASS CODE
REPRESENTING TWO-SEATER, COMPACT, MID-SIZE, ETC.,
     1      10     CITY-MPG         21       3    I      0     ESTIMATED (CITY) MPG OF THIS
MODEL TYPE (ROUNDED)
     1      11     HWY-MPG          24       3    I      0     HIGHWAY MPG OF THIS MODEL TYPE
(ROUNDED)
     1      12     COMB-MPG         27       3    I      0     COMBINED MPG OF THIS MODEL
TYPE (ROUNDED)
     1      13     FUEL-COST        30       6    I      0     ANNUAL FUEL COST BASED ON 15,000
MILES OF DRIVING PER YEAR
     1      14     DISP-CID         36       4    I      0     ENGINE DISPLACEMENT IN CUBIC
INCHES
     1      15     MODTRS           40       2    A      0     2-CHARACTER TRANSMISSION CODE -
SEE DATA FILE DESCRIPTION COMMENT #1
     1      16     FILLER           42       1    H      0     A HYPHEN I.E., -
     1      17     O-D-CODE         43       1    I      0     1=NO GEAR RATIO < 1, 2=TOP GEAR
RATO < 1, 3=ELECTRICALLY OPERATED OD
                                                               WHEN FUEL ECONOMY GUIDE REPORT IS
GENERATED).
     1      18     NO-CYL           44       2    I      0     NUMBER OF CYLINDERS
     1      19     FILLER           46       2    H      0     NOT USED
     1      20     FUEL-SYS         48       2    A      0     FUEL SYSTEM - 'FI' IF FUEL INJECTION,
# OF VETURIES FOR CARBURETORS
     1      21     MODTRN           50       1    A      0     1-CHARACTER TRANSMISSION CODE -
SEE DATA FILE DESCRIPTION COMMENT #1
     1      22     CATALYST         51       1    A      0     CATALYST APPLICATION : Y FOR
YES AND N FOR NO
     1      23     CITY-MPG-F       52       8    F      4     UNROUNDED MPG FOR CITY
DRIVING
     1      24     HWY-MPG-F        60       8    F      4     UNROUNDED MPG FOR HIGHWAY
DRIVING
     1      25     COMB-MPG-F       68       8    F      4     UNROUNDED MPG FOR CITY/HWY
COMBINED HARMONICALLY AVERAGED & WEIGHTED
     1      26     OPT-DISP         76       8    A      0     OPTIONAL DISPLACEMENT - BLANK,
(XXXXCC) OR (XX.XL)
     1      27     SALES-MTOT       84       6    I      0     SALES FOR MODEL LEVEL FUEL
ECONOMY CALCULATION
                                                               ERASED/BLANKED IF FOR PUBLIC ACCESS
     1      28     FUEL             90       2    I      0     FUEL TYPE: 6 & 7=UNLEADED GASOLINE, 
1 & 17=LEADED GASOLINE,
                                                                              9=DIESEL
     1      29     FILLER           92       3    H      0     NOT USED
     1      30     SALES-MTOTC      95       6    I      0     MODEL SALES EXCLUDING THOSEåWITH SUPPRESSION CODE 2 OR 9
                                                               ERASED/BLANKED IF FOR PUBLIC ACCESS
     1      31     FILLER          101      15    H      0     NOT USED
     1      32     CARLINE-NAME    116      28    A      0     CARLINE NAME DECODED FROM
5 DIGIT CARLINE CODE
     1      33     FILLER          144       4    H      0     NOT USED
     1      34     ENG-DSRPTR-1    148      10    A      0     BASIC ENGINE DESCRIPTOR 1
FROM CARD 1 INPUT
     1      35     ENG-DSRPTR-2    158      10    A      0     BASIC ENGINE DESCRIPTOR 2
FROM CARD 1 INPUT


[end]
