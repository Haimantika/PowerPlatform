## Abs-
 - Abs( Number )
 - Exp( Number )
 - Ln( Number )
 - Sqrt( Number )

Number - Required. Number to operate on.
 - Power( Base, Exponent )

Base - Required. Base number to raise.
Exponent - Required. The exponent to which the base number is raised.
 - Abs( SingleColumnTable )
 - Exp( SingleColumnTable )
 - Ln( SingleColumnTable )
 - Sqrt( SingleColumnTable )

SingleColumnTable - Required. A single-column table of numbers to operate on.
## Acceleration-
 - Acceleration.X	Right and left. Right is a positive number.
 - Acceleration.Y	Forward and back. Forward is a positive number.
 - Acceleration.Z	Up and down. Up is a positive number.
 - App.ActiveScreen	Screen that's showing. Returns a screen object, which you can use to reference properties of the screen or compare to another screen to determine which screen is showing. 
 - Compass.Heading	Heading in degrees. Returns a number 0 to 360, and 0 is north.
 - Connection.Connected	Returns a Boolean true or false value that indicates whether the device is connected to a network.
 - Connection.Metered	Returns a Boolean true or false value that indicates whether the connection is metered.
 - Location.Altitude	Returns a number that indicates the altitude, measured in feet, above sea level.
 - Location.Latitude	Returns a number, from –90 to 90, that indicates the latitude, as measured in degrees from the equator. A positive number indicates a location that's north of the equator.
 - Location.Longitude	Returns a number, from –180 to 180, that indicates the longitude, as measured in degrees from Greenwich, England. A positive number indicates a location that's east of Greenwhich.
 
## Acos,Acot-
 - Cos( Radians )
 - Cot( Radians )
 - Sin( Radians )
- Tan( Radians )

Radians - Required. Angle to operate on.
 - Cos( SingleColumnTable )
 - Cot( SingleColumnTable )
 - Sin( SingleColumnTable )
 - Tan( SingleColumnTable )

SingleColumnTable - Required. A single-column table of angles to operate on.
Inverse Functions
 - Acos( Number )
 - Acot( Number )
 - Asin( Number )
 - Atan( Number )

Number - Required. Number to operate on.
 - Acos( SingleColumnTable )
 - Acot( SingleColumnTable )
 - Asin( SingleColumnTable )
 - Atan( SingleColumnTable )

SingleColumnTable - Required. A single-column table of numbers to operate on.
Atan2( X, Y )

X - Required. X-axis coordinate.
Y - Required. Y-axis coordinate.
Helper Functions
Degrees( Radians )

Radians - Required. Angle in radians to convert to degrees.
Pi()

Radians( Degrees )

Degrees - Required. Angle in degrees to convert to radians.
## Add Columns
 - AddColumns( Table, ColumnName1, Formula1 [, ColumnName2, Formula2, ... ] )
 - DropColumns( Table, ColumnName1 [, ColumnName2, ... ] )
 - RenameColumns( Table, OldColumnName1, NewColumnName1 [, OldColumnName2, NewColumnName2, ... ] )
 - ShowColumns( Table, ColumnName1 [, ColumnName2, ... ] )
## And,Or,Not
 - And( x, y )
 - Or( x, y )	
 - Not( x )
## Assert
 - Assert(expression, message)

Expression – Required. An expression that evaluates to true or false.
Message – Not Required. A message that describes the assertion failure.

## Astype,Istype
 - AsType( RecordReference, EntityType )

RecordReference - Required. A record reference, often a lookup field that can refer to a record in any of multiple entities.
EntityType - Required. The specific entity for which to test.
 - IsType( RecordReference, EntityType )

RecordReference - Required. A record reference, often a lookup field that can refer to a record in any of multiple entities.
EntityType - Required. The specific entity to which the record should be cast.

## Average, Max, Min, StdevP, Sum, and VarP
 - Average( NumericalFormula1, [ NumericalFormula2, ... ] )
 - Max( NumericalFormula1, [ NumericalFormula2, ... ] )
 - Min( NumericalFormula1, [ NumericalFormula2, ... ] ) 
 - Sum( NumericalFormula1, [ NumericalFormula2, ... ] )
 - StdevP( NumericalFormula1, [ NumericalFormula2, ... ] )
 - VarP( NumericalFormula1, [ NumericalFormula2, ... ] )

NumericalFormula(s) - Required. Numeric values to operate on.
 - Average( Table, NumericalFormula )
 - Max( Table, NumericalFormula )
 - Min( Table, NumericalFormula )
 - Sum( Table, NumericalFormula )
 - StdevP( Table, NumericalFormula )
 - VarP( Table, NumericalFormula )

Table - Required. Table to operate on.
NumericalFormula - Required. Formula to evaluate for each record. The result of this formula is used for the aggregation. You can use columns of the table in the formula.
## Back and Navigate
 - Back( [ Transition ] )

Transition - Optional. The visual transition to use between the current screen and the previous screen. Refer to the list of valid values for this argument earlier in this article. By default, the transition through which a screen returns is the inverse of the transition through which it appeared.
 - Navigate( Screen [, Transition [, UpdateContextRecord ] ] )

Screen - Required. The screen to display.
Transition - Optional. The visual transition to use between the current screen and the next screen. See the list of valid values for this argument earlier in this article. The default value is None.
UpdateContextRecord - Optional. A record that contains the name of at least one column and a value for each column. 
## Blank, Coalesce, IsBlank, and IsEmpty
 - Coalesce( Value1 [, Value2, ... ] )

Value(s) – Required. Values to test. Each value is evaluated in order until a value that is not blank and not an empty string is found. Values after this point are not evaluated.
 - IsBlank( Value )

Value – Required. Value to test for a blank value or empty string.
 - IsEmpty( Table )

Table - Required. Table to test for records.
## Calendar and Clock
 - Calendar.MonthsLong()
 - Calendar.MonthsShort()
 - Calendar.WeekdaysLong()
 - Calendar.WeekdaysShort()
 - Clock.AmPm()
 - Clock.AmPmShort()
 - Clock.IsClock24()
## Char
 - Char( CharacterCode )

CharacterCode - Required. ASCII character code to translate.
## Choices
 - Choices( column-reference )

column-reference – Required. A lookup column of a data source. Don't enclose the column name in double quotes. The reference must be directly to the column of the data source and not pass through a function or a control.
## Collect, Clear, and ClearCollect
 - Collect( DataSource, Item, ... )

DataSource – Required. The data source that you want to add data to. If it doesn't already exist, a new collection is created.
Item(s) - Required. One or more records or tables to add to the data source.
 - Clear( Collection )

Collection – Required. The collection that you want to clear.
 - ClearCollect( Collection, Item, ... )

Collection – Required. The collection that you want to clear and then add data to.
Item(s) - Required. One or more records or tables to add to the data source.
## Color enumeration and ColorFade, ColorValue, and RGBA 
 - Color.ColorName

ColorName - Required. A Cascading Style Sheet (CSS) color name. The list of possible enumeration values appears at the end of this topic.
ColorValue( CSSColor )

 - CSSColor - Required. A Cascading Style Sheet (CSS) color definition. You can specify either a name, such as OliveDrab, or a hex value, such as #6b8e23 or #7fffd420. Hex values can take the form of either #rrggbb or #rrggbbaa.
 - RGBA( Red, Green, Blue, Alpha )

Red, Green, Blue - Required. Color-component values, which range from 0 (no saturation) to 255 (full saturation).
Alpha - Required. Alpha component, which ranges from 0 (fully transparent) to 1 (fully opaque). You can also use a percentage, 0% to 100%.
ColorFade( Color, FadeAmount )

Color - Required. A color value such as Color.Red or the output from ColorValue or RGBA.
FadeAmount - Required. A number between -1 and 1. -1 fully darkens a color to black, 0 doesn't affect the color, and 1 fully brightens a color to white. You can also use a percentage from -100% to 100%.
## Concat and Concatenate 
 - Concat( Table, Formula )

Table - Required. Table to operate on.
Formula - Required. Formula to apply across the records of the table.
 - Concatenate( String1 [, String2, ...] )

String(s) - Required. Mix of individual strings or a single-column table of strings.
## Concurrent
 - Concurrent( Formula1, Formula2 [, ...] )

Formula(s) – Required. Formulas to evaluate concurrently. You must supply at least two formulas.
## Count, CountA, CountIf, and CountRows
 - Count( SingleColumnTable )
 - CountA( SingleColumnTable )

SingleColumnTable - Required. Column of records to count.
 - CountIf( Table, LogicalFormula )

Table - Required. Table of records to count.
LogicalFormula - Required. Formula to evaluate for each record of the table. Records that return true for this formula are counted. The formula can reference columns of the table.
CountRows( Table )

Table - Required. Table of records to count.
