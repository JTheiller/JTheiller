# pascal-format-datetime

Um `TDateTime` por ser `formatado` como texto conforme necessidade, utilizando as `configurações regionais padrões do sistema operacional`, podendo ser redefinido com terceiro parametro `TFormatSettings`.

## Uso
- Uses: `System.SysUtils`
- Sintaxe: `FormatDateTime(maskString, date, TFormatSettings)`
- Code: `FormatDateTime('dd/MM/yy hh:mm:ss', TDateTime.Now, newFormatSettings)`
- Result: `27/04/22 00:41:12`

## Definições TFormatSettings
```
  DateSeparator      := '-';
  TimeSeparator      := '_';
  ShortDateFormat    := 'dd/mmm/yy';
  LongDateFormat     := 'dddd dd of mmmm of yyyy';
  TimeAMString       := 'morning';
  TimePMString       := 'afternoon';
  ShortTimeFormat    := 'hh:nn:ss';
  LongTimeFormat     := 'hh : nn : ss . zzz';
  ShortMonthNames[6] := 'JUN';
  LongMonthNames[6]  := 'JUNE';
  ShortDayNames[1]   := 'SUN';
  LongDayNames[1]    := 'SUNDAY';
  TwoDigitYearCenturyWindow := 75;
```
## Examples
```
   dd/mm/yy hh:mm:ss = 05/06/49 01:02:03
                 mmm = Jun
                mmmm = June
                 ddd = Sat
                dddd = Saturday
               ddddd = 05/06/2049
              dddddd = 05 June 2049
              hhampm = 01AM
                   t = 01:02
                  tt = 01:02:03
          dd/mm/yyyy = 05/06/2049
  
   dd/mm/yy hh:nn:ss = 05-06-49 01_02_03
                 mmm = JUN
                mmmm = JUNE
                 ddd = SUN
                dddd = SUNDAY
               ddddd = 05-JUN-49
              dddddd = SUNDAY 05 of JUNE of 1949
              hhampm = 01morning
                   t = 01_02_03
                  tt = 01 _ 02 _ 03 . 004
          dd/mm/yyyy = 05-06-1949
 ```
