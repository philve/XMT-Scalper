#XMT-Scalper

Translation of the XMT Scalper robot into CSharp from its source in Mql4.

# XMT-Scalper origin

'XMT-Scalper' is a robot i.e. a computer program or Expert Advisor (EA) running on the MetaTrader 4 trading platform
It originally originated from a preliminary version of a trading robot named 'MillionDollarPips' but it has been extensively enhanced and improved.
Today, all the code has been rewritten from scratch, and only part of the strategy's core is identical to its base version.
This EA is not a commercial product, but is available for free.

# Objectives

The Initial Project of a scalping trading robot XMT-Scalper v2.4.6.1 written in MQL4 comes from [Capella](http://www.worldwide-invest.org).
It was translated into CSharp by [Abdallah Hacid](ab.hacid@gmail.com) with the help of the [NQuotes](http://www.nquotes.net/) library of [Daniel](support2@nquotes .net).
From there we propose to restructure the code to make it more modular and thus more readable and then to make it evolve more
merely.

# Advantages
An undeniable advantage of the NQuotes system is that you can write indicators and trading robots in CSharp and execute them directly
on the MetaTrader 4 platform, you can also debug or control the robot from a Windows Form or WPF interface.

# Installation

To compile the program with Visual Studio, you must first:

1) install [metatrader 4](http://www.metatrader4.com/).

2) install [NQuotes](http://www.nquotes.net/installation)

3) Modify post-buids instructions of both MqlApiWithStdLib and XMT-Scalper projects
  
   replace in 'xcopy "$(ProjectDir)$(OutDir)$(TargetFileName)" "C:\Users\{user}\AppData\Roaming\MetaQuotes\Terminal\{key}\MQL4\Experts" /Y'

   a) your own unique metatrader 4 installation key which can be found in the '%TERMINAL_DATA_PATH%' directory located in
   C:\Users\{user}\AppData\Roaming\MetaQuotes\Terminal\.
  
   b) your windows username.

# Debugging with NQuotes

   To debug the program with NQuotes follow the [instructions](http://www.nquotes.net/expert-creation-tutorial) given by its author [Daniel](support2@nquotes.net ).

#Notes
  
   a) if metatrader is active, there is an error during compilation (dll copying is not done) because the dlls are blocked in access by metratrader.
