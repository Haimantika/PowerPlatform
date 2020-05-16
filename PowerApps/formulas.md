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
## DataSourceInfo 
 - DataSourceInfo( DataSource, Information, ColumnName )

DataSource – Required. The data source to use.

Information – Required. The type of information that you want to retrieve.

ColumnName – Optional. For column-level information, the column name as a string. Column Phone would be passed as "Phone", including the double quotes. For information at the data-source level, the ColumnName argument can't be used.
## Date and Time 
 - Date( Year, Month, Day )

Year - Required. Numbers greater than 1899 are interpreted as absolute (1980 is interpreted as 1980); numbers that range from 0 to 1899 are interpreted as relative to 1900. (For example, 80 is interpreted as 1980.)
Month - Required. A number that ranges from 1 to 12.
Day - Required. A number that ranges from 1 to 31.
 - Time( Hour, Minute, Second )

Hour - Required. A number that ranges from 0 (12:00 AM) to 23 (11:00 PM).
Minute - Required. A number that ranges from 0 to 59.
Second - Required. A number that ranges from 0 to 59.
## DateAdd, DateDiff, and TimeZoneOffset
 - DateAdd( DateTime, Addition [, Units ] )

DateTime - Required. Date/time value to operate on.
Addition - Required. Number, in Units, to add to the DateTime.
Units - Optional. The type of Units to add: Milliseconds, Seconds, Minutes, Hours, Days, Months, Quarters, or Years. If not specified, Days are used.
 - DateDiff( StartDateTime, EndDateTime [, Units ] )

StartDateTime - Required. Starting date/time value.
EndDateTime - Required. Ending date/time value.
Units - Optional. The type of Units to add: Milliseconds, Seconds, Minutes, Hours, Days, Months, Quarters, or Years. If not specified, Days are used.
 - TimeZoneOffset( [ DateTime ] )

DateTime - Optional. Date/time value for which to return the offset. By default, the current date/time is used.
## DateValue, TimeValue, and DateTimeValue
 - DateValue( String [, Language ])
 - DateTimeValue( String [, Language ])
 - TimeValue( String [, Language ])

String - Required. A text string that contains a date, time, or combination date and time value.
Language - Optional. A language string, such as would be returned by the first two characters from the Language function. If not provided, the language of the current user's settings is used.
## Day, Month, Year, Hour, Minute, Second, and Weekday
 - Day( DateTime )
 - Month( DateTime )
 - Year( DateTime )
 - Hour( DateTime )
 - Minute( DateTime )
 - Second( DateTime )

DateTime - Required. Date/Time value to operate on.
 - Weekday( DateTime [, WeekdayFirst ] )

DateTime - Required. Date/Time value to operate on.
WeekdayFirst - Optional. Excel code specifying which day starts the week. If not supplied, 1 (Sunday first) is used.
## Defaults
 - Defaults( DataSource )

DataSource – Required. The data source for which you want default values.
## Enable and Disable
 - Enable( Signal )
 - Disable( Signal )

Signal - Required. The signal to turn on or off.
## Distinct
 - Distinct( Table, Formula )

Table - Required. Table to evaluate across.
Formula - Required. Formula to evaluate for each record.
## Download
 - Download( Address )

Address – Required. The URL address of a web resource to download.
## EditForm, NewForm, SubmitForm, ResetForm, and ViewForm
 - SubmitForm( FormName )

FormName - Required. Form control to submit to the data source.
 - EditForm( FormName )

FormName - Required. Form control to switch to FormMode.Edit mode.
 - NewForm( FormName )

FormName - Required. Form control to switch to FormMode.New mode.
 - ResetForm( FormName )

FormName - Required. Form control to reset to initial values. Also switches the form from FormMode.New mode to FormMode.Edit mode.
 - ViewForm( FormName )

FormName - Required. Form control to switch to FormMode.View mode.
## EndsWith and StartsWith
 - EndsWith( Text, EndText )

Text – Required. The text to test.
EndText – Required. The text to search for at the end of Text. If EndText is an empty string, EndsWith returns true.
 - StartsWith( Text, StartText )

Text – Required. The text to test.
StartText – Required. The text to search for at the beginning of Text. If StartText is an empty string, StartsWith returns true.
## Errors
 - Errors( DataSource [, Record ] )

DataSource – Required. The data source for which you want to return errors.
Record – Optional. A specific record for which you want to return errors. If you don't specify this argument, the function returns errors for the entire data source.
## EncodeUrl and PlainText
 - EncodeUrl( String )

String - Required. URL to be encoded.
 - PlainText( String )

String - Required. String from which HTML and XML tags will be stripped.
## Exit
 - Exit( [Signout] )

Signout – Optional. A Boolean value that if true will sign the current user out of Power Apps. The default is false and the user remains signed in.
## Filter, Search, and LookUp
 - Filter( Table, Formula1 [, Formula2, ... ] )

Table - Required. Table to search.
Formula(s) - Required. The formula by which each record of the table is evaluated. The function returns all records that result in true. You can reference columns within the table. If you supply more than one formula, the results of all formulas are combined with the And function.
 - Search( Table, SearchString, Column1 [, Column2, ... ] )

Table - Required. Table to search.
SearchString - Required. The string to search for. If blank or an empty string, all records are returned.
Column(s) - Required. The names of columns within Table to search. Columns to search must contain text. Column names must be strings and enclosed in double quotes. However, the column names must be static and cannot be calculated with a formula. If SearchString is found within the data of any of these columns as a partial match, the full record will be returned.
 - LookUp( Table, Formula [, ReductionFormula ] )

Table - Required. Table to search. In the UI, the syntax is shown as source above the function box.
Formula - Required. The formula by which each record of the table is evaluated. The function returns the first record that results in true. You can reference columns within the table. In the UI, the syntax is shown as condition above the function box.
ReductionFormula - Optional. This formula is evaluated over the record that was found, and then reduces the record to a single value. You can reference columns within the table. If you don't use this parameter, the function returns the full record from the table. In the UI, the syntax is shown as result above the function box.
## Find
 - Find( FindString, WithinString [, StartingPosition ] )

FindString - Required. The string to find.
WithinString - Required. The string to search within.
StartingPosition - Optional. The starting position to start searching. Position 1 is the first character.
## First, FirstN, Last, and LastN
 - First( Table )
 - Last( Table )

Table - Required. Table to operate on.
 - FirstN( Table [, NumberOfRecords ] )
 - LastN( Table [, NumberOfRecords ] )

Table - Required. Table to operate on.
NumberOfRecords - Optional. Number of records to return. If you don't specify this argument, the function returns one record.

## ForAll
 - ForAll( Table, Formula )

Table - Required. Table to be acted upon.
Formula - Required. The formula to evaluate for all records of the Table.
## GroupBy and Ungroup
 - GroupBy( Table, ColumnName1 [, ColumnName2, ... ], GroupColumnName )

Table - Required. Table to be grouped.

ColumnName(s) - Required. The column names in Table by which to group records. These columns become columns in the resulting table.

GroupColumnName - Required. The column name for the storage of record data not in the ColumnName(s).
 - Ungroup( Table, GroupColumnName )

Table - Required. Table to be ungrouped.

GroupColumnName - Required. The column that contains the record data setup with the GroupBy function.
## GUID
 - GUID( [ GUIDString ] )

GUIDString – Optional. A text string that contains the hexadecimal representation of a GUID. If no string is supplied, a new GUID is created.
## HashTags
 - HashTags( String )

String - Required. String to scan for hashtags.
## If and Switch
 - If( Condition, ThenResult [, DefaultResult ] )
If( Condition1, ThenResult1 [, Condition2, ThenResult2, ... [ , DefaultResult ] ] )

Condition(s) - Required. Formula(s) to test for true. Such formulas commonly contain comparison operators (such as <, >, and =) and test functions such as IsBlank and IsEmpty.
ThenResult(s) - Required. The corresponding value to return for a condition that evaluates to true.
DefaultResult - Optional. The value to return if no condition evaluates to true. If you don't specify this argument, blank is returned.
 - Switch( Formula, Match1, Result1 [, Match2, Result2, ... [, DefaultResult ] ] )

Formula - Required. Formula to evaluate for matches. This formula is evaluated only once.
Match(s) - Required. Values to compare with the result from Formula. If an exact match is found, the corresponding Result is returned.
Result(s) - Required. The corresponding value to return when an exact match is found.
DefaultResult - Optional. If an exact match isn't found, this value is returned. If you don't specify this argument, blank is returned.
## IfError and IsError
 - IfError( Value1, Replacement1 [, Value2, Replacement2, ... [, DefaultResult ] ] )

Value(s) – Required. Formula(s) to test for an error value.
Replacement(s) – Required. The formulas to evaluate and values to return if matching Value arguments returned an error.
DefaultResult – Optional. The formulas to evaluate if the formula doesn't find any errors.
 - IsError( Value )

Value – Required. Formula to test for an error value.
## IsMatch, Match, and MatchAll
 - IsMatch( Text, Pattern [, Options ] )

Text – Required. The text string to test.
Pattern – Required. The pattern to test as a text string. Concatenate predefined patterns that the Match enum defines, or provide a regular expression. Pattern must be a constant formula without any variables, data sources, or other dynamic references that change as the app runs.
Options – Optional. A text-string combination of MatchOptions enum values. By default, MatchOptions.Complete is used.
 - Match( Text, Pattern [, Options ] )

Text – Required. The text string to match.
Pattern – Required. The pattern to match as a text string. Concatenate predefined patterns that the Match enum defines, or provide a regular expression. Pattern must be a constant formula without any variables, data sources, or other dynamic references that change as the app runs.
Options – Optional. A text-string combination of MatchOptions enum values. By default, MatchOptions.Contains is used.
 - MatchAll( Text, Pattern [, Options ] )

Text – Required. The text string to match.
Pattern – Required. The pattern to match as a text string. Concatenate predefined patterns that the Match enum defines, or provide a regular expression. Pattern must be a constant formula without any variables, data sources, or other dynamic references that change as the app runs.
Options – Optional. A text-string combination of MatchOptions enum values. By default, MatchOptions.Contains is used.
## IsNumeric
 - IsNumeric( Value )

Value – Required. Value to test.
## Now, Today, and IsToday
 - Now()

 - Today()

 - IsToday( DateTime )

DateTime - Required. The date/time value to test.
## JSON
 - JSON( DataStructure [, Format ] )

DataStructure – Required. The data structure to convert to JSON. Tables, records, and primitive values are supported, arbitrarily nested.
Format - Optional. JSONFormat enum value. The default value is Compact, which doesn't add newlines or spaces and blocks binary data and unsupported columns.
## Language - The Language function returns the language, script, and region of the current user as a language tag.
 - Language()
 ## Left, Mid, and Right
  - Left( String, NumberOfCharacters )
 - Mid( String, StartingPosition [, NumberOfCharacters ] )
 - Right( String, NumberOfCharacters )

String - Required. The string to from which to extract the result.
StartingPosition - Required (Mid only). The starting position. The first character of the string is position 1.
NumberOfCharacters - Required (Left and Right only). The number of characters to return. If omitted for the Mid function, the function returns the portion from the starting position until the end of the string.
 - Left( SingleColumnTable, NumberOfCharacters )
 - Mid( SingleColumnTable, StartingPosition [, NumberOfCharacters ] )
 - Right( SingleColumnTable, NumberOfCharacters )

SingleColumnTable - Required. A single-column table of strings from which to extract the results.
StartingPosition - Required (Mid only). The starting position. The first character of the string is position 1.
NumberOfCharacters - Required (Left and Right only). The number of characters to return. If omitted for the Mid function, the function returns the portion from the starting position until the end of the string.
## Len
 - Len( String )

String - Required. The string to measure.
 - Len( SingleColumnTable )

SingleColumnTable - Required. A single-column table of strings to measure.
## SaveData and LoadData
 - SaveData( Collection, Name )
 - LoadData( Collection, Name [, IgnoreNonexistentFile ])

Collection - Required. Collection to be stored or loaded.
Name - Required. Name of the storage. The name must be same to save and load same set of data. The name space isn't shared with other apps or users. Names must not contain any of these characters: *".?:\<>|/.
IgnoreNonexistentFile - Optional. A Boolean value indicating what to do if the file doesn't already exist. Use false (default) to return an error and true to suppress the error.

## Lower, Upper, and Proper 
 - Lower( String )
 - Upper( String )
 - Proper( String )

String - Required. The string to convert.
 - Lower( SingleColumnTable )
 - Upper( SingleColumnTable )
 - Proper( SingleColumnTable )

SingleColumnTable - Required. A single-column table of strings to convert.
## Mod
 - Mod( Number, Divisor )

Number - Required. Number to divide.
Divisor - Required. Number to divide by.
## Notify
 - Notify( Message [, NotificationType [ , Timeout ] ] )

Message – Required. Message to display to the user.
NotificationType – Optional. Type of the message to display from the table above. The default is NotificationType.Information.
Timeout – Optional. Number of milliseconds to wait before automatically dismissing the notification. The default is 10 seconds (or 10,000 milliseconds). The notification will be displayed indefinitely with a Timeout of 0.
## Patch
 - Modify or create a record in a data source
 - Patch( DataSource, BaseRecord, ChangeRecord1 [, ChangeRecord2, … ])

DataSource – Required. The data source that contains the record that you want to modify or will contain the record that you want to create.
BaseRecord – Required. The record to modify or create. If the record came from a data source, the record is found and modified. If the result of Defaults is used, a record is created.
ChangeRecord(s) – Required. One or more records that contain properties to modify in the BaseRecord. Change records are processed in order from the beginning of the argument list to the end, with later property values overriding earlier ones.
 - Modify or create a set of records in a data source
 - Patch( DataSource, BaseRecordsTable, ChangeRecordTable1 [, ChangeRecordTable2, … ] )

DataSource – Required. The data source that contains the records that you want to modify or will contain the records that you want to create.
BaseRecordTable – Required. A table of records to modify or create. If the record came from a data source, the record is found and modified. If the result of Defaults is used, a record is created.
ChangeRecordTable(s) – Required. One or more tables of records that contain properties to modify for each record of the BaseRecordTable. Change records are processed in order from the beginning of the argument list to the end, with later property values overriding earlier ones.
 - Merge records
 - Patch( Record1, Record2 [, …] )

Record(s) - Required. At least two records that you want to merge. Records are processed in order from the beginning of the argument list to the end, with later property values overriding earlier ones.
## Rand - Returns a pseudo-random number.
 - Rand()
 ## Refresh
  - Refresh( DataSource )

DataSource – Required. The data source that you want to refresh.
## Relate and Unrelate
 - Relate( Entity1RelatedTable, Entity2Record )

Entity1RelatedTable - Required. For a record of Entity1, the table of Entity2 records related through a one-to-many or many-to-many relationship.
Entity2Record - Required. The Entity2 record to add to the relationship.
 - Unrelate( Entity1RelatedTable, Entity2Record )

Entity1RelatedTable - Required. For a record of Entity1, the table of Entity2 records related through a one-to-many or many-to-many relationship.
Entity2Record - Required. The Entity2 record to remove from the relationship.
## Remove and RemoveIf
 - Remove( DataSource, Record1 [, Record2, ... ] [, All ] )

DataSource – Required. The data source that contains the record or records that you want to remove.
Record(s) – Required. The record or records to remove.
All – Optional. In a collection, the same record may appear more than once. You can add the All argument to remove all copies of the record.
 - Remove( DataSource, Table [, All ] )

DataSource – Required. The data source that contains the records that you want to remove.
Table – Required. A table of records to remove.
All – Optional. In a collection, the same record may appear more than once. You can add the All argument to remove all copies of the record.
 - RemoveIf( DataSource, Condition [, ... ] )

DataSource – Required. The data source that contains the record or records that you want to remove.
Condition(s) – Required. A formula that evaluates to true for the record or records to remove. You can use column names from the DataSource in the formula. If you specify multiple Conditions, all must evaluate to true for the record or records to be removed.
## Replace and Substitute
 - Replace( String, StartingPosition, NumberOfCharacters, NewString )

String - Required. The string to operate on.
StartingPosition - Required. Character position to start the replacement. The first character of String is at position 1.
NumberOfCharacters - Required. The number of characters to replace in String.
NewString - Required. The replacement string. The number of characters in this argument can differ from the NumberOfCharacters argument.
 - Substitute( String, OldString, NewString [, InstanceNumber ] )

String - Required. The string to operate on.
OldString - Required. The string to replace.
NewString - Required. The replacement string. OldString and NewString can have different lengths.
InstanceNumber - Optional. Use this argument to specify which instance of OldString to replace if String contains more than one instance. If you don't specify this argument, all instances will be replaced.
 - Replace( SingleColumnTable, StartingPosition, NumberOfCharacters, NewString )

SingleColumnTable - Required. A single-column table of strings to operate on.
StartingPosition - Required. Character position to start the replacement. The first character of each string in the table is at position 1.
NumberOfCharacters - Required. The number of characters to replace in each string.
NewString - Required. The replacement string. The number of characters in this argument can differ from the NumberOfCharacters argument.
 - Substitute( SingleColumnTable, OldString, NewString [, InstanceNumber ] )

SingleColumnTable - Required. A single-column table of strings to operate on.
OldString - Required. The string to replace.
NewString - Required. The replacement string. OldString and NewString can have different lengths.
InstanceNumber - Optional. Use this argument to specify which instance of OldString to replace if String contains more than one instance. If you don't specify this argument, all instances will be replaced.
## Reset
 - Reset( Control )

Control – Required. The control to reset.
## Revert
 - Revert( DataSource [, Record ] )

DataSource – Required. The data source that you want to revert.
Record - Optional. The record that you want to revert. If you don't specify a record, the entire data source is reverted.
## Round, RoundDown, and RoundUp
 - Round( Number, DecimalPlaces )
 - RoundDown( Number, DecimalPlaces )
 - RoundUp( Number, DecimalPlaces )

Number - Required. The number to round.
DecimalPlaces - Required. The number of places to the right of the decimal point to round to. Use 0 to round to a whole number.
## Select
 - Select( Control )

Control – Required. The control to select on behalf of the user.
 - Select( Control, Row or column, Child Control )

Control – Required. The control to select on behalf of the user.
Row or column – Not required. The number of row or column (starting with 1) in a gallery control to select on behalf of the user.
Child Control - Not required. The child control of the control identified in the 'control' parameter to select.
## Set
 - Set( VariableName, Value )

VariableName - Required. The name of a global variable to create or update.
Value - Required. The value to assign to the context variable.
## SetFocus
 - SetFocus( Control )

Control – Required. The control to give the input focus.
## SetProperty
 - SetProperty(Control Property, value)

Control Property – Required. The control property to set on behalf of the user.
Value – Required. The value of the property to set on behalf of the user.
## Shuffle
 - Shuffle( Table )

Table - Required. Table to shuffle.
## Sort and SortByColumns
 - Sort( Table, Formula [, SortOrder ] )

Table - Required. Table to sort.
Formula - Required. This formula is evaluated for each record of the table, and the results are used to sort the table. You can reference columns within the table.
SortOrder - Optional. Specify SortOrder.Descending to sort the table in descending order. SortOrder.Ascending is the default value.
 - SortByColumns( Table, ColumnName1 [, SortOrder1, ColumnName2, SortOrder2, ... ] )

Table - Required. Table to sort.

ColumnName(s) - Required. The column names to sort on, as strings.

SortOrder(s) - Optional. SortOrder.Ascending or SortOrder.Descending. SortOrder.Ascending is the default. If multiple ColumnNames are supplied, all but the last column must include a SortOrder.
 - SortByColumns( Table, ColumnName, SortOrderTable )

Table - Required. Table to sort.

ColumnName - Required. The column name to sort on, as strings.

SortOrderTable - Required. Single column table of values to sort by.

## Split
 - Split( Text, Separator )

Text - Required. Text to split.
Separator - Required. Separator to use in splitting the string. Can be zero, one, or more characters.
## Table
 - Table( Record1 [, Record2, ... ] )

Record(s) - Required. The records to add to the table.
## Text
 - Text( NumberOrDateTime, DateTimeFormatEnum [, ResultLanguageTag ] )

NumberOrDateTime - Required. The number or the date/time value to format.
DateTimeFormat - Required. A member of the DateTimeFormat enumeration.
ResultLanguageTag - Optional. The language tag to use for the result text. By default, the language of the current user is used.
 - Text( NumberOrDateTime, CustomFormat [, ResultLanguageTag ] )

Number - Required. The number or the date/time value to format.
CustomFormat - Required. One or more placeholders enclosed in double quotation marks.
ResultLanguageTag - Optional. The language tag to use for the result text. By default, the language of the current user is used.
 - Text( AnyValue )

AnyValue - Required. Value to convert to a text representation. A default format is used.
## Trace 
 - Trace(message, trace_severity, custom_record )

Message – Required. The information to be traced. In tests, this creates a record in the Traces table in the TestCaseResult record.
Trace_severity - Optional. The severity level of the Trace recorded in Application Insights. Options are TraceSeverity.Information, TraceSeverity.Warning or TraceSeverity.Error.
custom_record - Optional. A record containing custom data that will be recorded in Application Insights.
## Trim and TrimEnds
 - Trim( String )
 - TrimEnds( String )

String - Required. The string of text to remove spaces from.
 - Trim( SingleColumnTable )
 - TrimEnds( SingleColumnTable )

SingleColumnTable - Required. A single-column table of strings to remove spaces from.
## Update and UpdateIf
 - Update( DataSource, OldRecord, NewRecord [, All ] )

DataSource – Required. The data source that contains the record that you want to replace.
OldRecord – Required. The record to replace.
NewRecord – Required. The replacement record. This isn't a change record. The entire record is replaced, and missing properties will contain blank.
All – Optional. In a collection, the same record may appear more than once. Specify the All argument to remove all copies of the record.
 - UpdateIf( DataSource, Condition1, ChangeRecord1 [, Condition2, ChangeRecord2, ... ] )

DataSource – Required. The data source that contains the record or records that you want to modify.
Condition(s) – Required. A formula that evaluates to true for the record or records that you want to modify. You can use column names of DataSource in the formula.
ChangeRecord(s) - Required. For each corresponding condition, a change record of new property values to apply to records of DataSource that satisfy the condition. If you provide the record inline using curly braces, property values of the existing record can be used in the property formulas.
## UpdateContext
 - UpdateContext( UpdateRecord )

UpdateRecord – Required. A record that contains the name of at least one column and a value for that column. A context variable is created or updated for each column and value that you specify.
 - UpdateContext( { ContextVariable1: Value1 [, ContextVariable2: Value2 [, ... ] ] } )

ContextVariable1 - Required. The name of a context variable to create or update.
Value1 - Required. The value to assign to the context variable.
ContextVariable2: Value2, ... - Optional. Additional context variables to create or update and their values.
## User - The User function returns a record of information about the current user:
 - User()
## Validate
 - Validate( DataSource, Column, Value )

DataSource – Required. The data source to validate with.
Column – Required. The column to validate.
Value – Required. The value for the selected column to be validated.
Validate( DataSource, OriginalRecord, Updates )

DataSource – Required. The data source to validate with.
OriginalRecord - Required. The record to which updates are to be validated.
Updates - Required. The changes to apply to the original record.
## Value
 - Value( String [, LanguageTag ] )

String - Required. String to convert to a numeric value.
LanguageTag - Optional. The language tag in which to parse the string. If not specified, the language of the current user is used.
## With 
 - With( Record, Formula )

Record – Required. The record to be acted upon. For names values, use the inline syntax { name1: value1, name2: value2, ... }
Formula – Required. The formula to evaluate for Record. The formula can reference any of the fields of Record directly as a record scope.
