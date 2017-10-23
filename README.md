Voip <dot> MS is a service provider for VoIP calling, SMS, and eFax.

The program 'vms' uses the Voip::MS package to use their api to make
basic calls.

Demo'ed initially are 'getBalance' and 'getCDR' though more fleshing will
happen eventually.

vms [-c <config>] -p <personality> [-n]
  <config> = config file
  <personality> = action to take, implemented actions are:
	balance
	CDR -f <fromdate> -t <todate>
	servers
	internationalinfo
	callaccounts = show registration status of voip clients
	billing = billing types (all, free, billed .. by default)
	calltypes = in/out various paths
	regstatus
	packages
	dids
	sendsms [-f <sms did>] [-t <sms dst>] -m "message to send"
	smslist [-f <fromdate>] [-t <todate>]
