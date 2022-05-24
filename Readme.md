## Plan Check June 22 , 06/11, Fortaleza, Brazil 

### João Henrique Martins Castelo and Anselmo Mancini 

#### We need 5 checks
	[X] - Check if Dicom Origin was changed by an user
		How ? 
		[X] - Origin is 0,0,0 if not changed
	[X] - Check if there is a Setup Field in the Plan
		How ?
		[X] - Check Setup property in the field
	[X] - Check if MU Factor is larger than 7
		How ?
		[X] - Sum all fields MUs and divide it by the dose per fraction in cGy
	[] - Check the primary reference point dose 
		How ?
		[] Check Prescription and Dose Information
		[] Dose per day and per session = Total Dose/ nbOfFractions
		[] Rounding is important here
	[] - Match PTV D95 with Doctor prescription
		How ?
		[] Loop on RT Prescription
		[] Loop PTV List
		[] Check if D95 is within Prescription 90-100% 
		[] Match PTVs and report to the User 🚀

