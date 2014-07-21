TimeChange
==========

An Event Extension module for JC2-MP
	--						TimeChange	--	Event Extension					--
	--
	--	TimeChange is a backend module designed to be loaded and let run.
	--	TimeChange adds two events to both Server and Client, These events are:
	--	"TimeChange" and "SecondTick"
	--	Both contain a table.
	--	
	--	----------					"TimeChange" contains:					----------
	--	Name					Always contained:		Type:			Description:
	--	args.Minute				Yes						Number(0-59)	The current minute
	--	args.Hour				Yes						Number(0-23)	The current hour
	--	args.FifthMinute		No						Bool			If the event happened on a minute divisible by 5
	--	args.TenthMinute		No						Bool			If the event happened on a minute divisible by 10
	--	args.FifteenthMinute	No						Bool			If the event happened on a minute divisible by 15
	--	args.HalfHour			No						Bool			If the event happened on a halfhour(beginning or middle of the hour)
	--	args.HourChange			No						Bool			If the hour has changed.
	--	args.QuarterDaily		No						Bool			If the hour is a quarter of the day(Happens at 0, 6, 12, and 18 hours)
	--	args.DayChange			No						Bool			If the day has changed(Happens at midnight).
	--	
	--	----------					"SecondTick" contains:					----------
	--	Name					Always contained:		Type:			Description:
	--	args.Second				Yes						Number(0-59)	The current second
	--	args.Even				Yes						Bool			True or False if the second is even.
	--	
