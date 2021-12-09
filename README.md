# Online VIN decoder - command line access

This is an example of command line access to VinLink online VIN decoder.

You need to create an account at www.vinlink.com

It's necessary to add some money for production use of service however you may apply for free funds for tests.

You may decode a sample VIN using command line tools like curl or wget
```
curl -s -u "login: password" --digest -o 1FMCU04112KA71263.xml "http://service.vinlink.com/report?type=BASIC_PLUS&vin=1FMCU04112KA71263"
```
or
```
wget --http-user=login --http-password=password -q -O 1FMCU04112KA71263.xml "http://service.vinlink.com/report?type=BASIC_PLUS&vin=1FMCU04112KA71263"
```
Decode result will be saved to requested 1FMCU04112KA71263.xml file

```
<?xml version="1.0" encoding="UTF-8" ?>
<REPORTS>
	<REPORT type="BASIC_PLUS">
		<VINPOWER
			version="PASSENGER, MPV, LIGHT TRUCK 2021 12.002; TRUCKS FILE 2021 12.002; PASSENGER, MPV, LIGHT TRUCK 2021 12.002; OTHER PASSENGER VEHICLES 2021 12.002; MOTORCYCLES FILE 2021 12.002; TRAILERS 2021 12.002; TRAILERS 2021 12.002;">
			<DATABASE version="2021.12.002">
				<MODULE name="PASSENGER, MPV, LIGHT TRUCK"
					version="2021.12.002" />
				<MODULE name="TRUCKS FILE" version="2021.12.002" />
				<MODULE name="PASSENGER, MPV, LIGHT TRUCK"
					version="2021.12.002" />
				<MODULE name="OTHER PASSENGER VEHICLES" version="2021.12.002" />
				<MODULE name="MOTORCYCLES FILE" version="2021.12.002" />
				<MODULE name="TRAILERS" version="2021.12.002" />
				<MODULE name="TRAILERS" version="2021.12.002" />
			</DATABASE>
			<VIN number="1FMCU04112KA71263">
				<DECODED Model_Year="2002" Make="Ford" Model="Escape">
					<ITEM name="Model Year" value="2002" />
					<ITEM name="Make" value="Ford" />
					<ITEM name="Model" value="Escape" />
					<ITEM name="Trim Level" value="XLT" />
					<ITEM name="Body Type" value="4 Door Wagon" />
					<ITEM name="Manufacturer" value="Ford Motor Company" />
					<ITEM name="Production Seq. Number" value="A71263" />
					<ITEM name="Engine Type" value="V6, 3.0L; DOHC 24V; SEFI" />
					<ITEM name="Engine Manufacturer" value="Ford" />
					<ITEM name="Fuel Type" value="Gasoline" />
					<ITEM name="Horsepower" value="201HP" />
					<ITEM name="Engine Code" value="1" />
					<ITEM name="Drive Line Type" value="4WD" />
					<ITEM name="Vehicle Type" value="Multipurpose Vehicle (MPV)" />
					<ITEM name="Vehicle Class" value="Small MPV" />
					<ITEM name="Brake System" value="Hydraulic" />
					<ITEM name="Restraint System"
						value="Side Air Bag; Air Bag-2nd Generation" />
					<ITEM name="Country" value="UNITED STATES" />
					<ITEM name="Assy. Plant" value="Kansas City: Claycomo, MO" />
					<ITEM name="GVWR Class" value="Class C: 4,001-5,000 lb" />
					<ITEM name="Tonnage" value="1/2" />
					<ITEM name="Check Digit" value="1" />
					<ITEM name="MPG" value="A4:16-22-18" />
					<ITEM name="AAIA" value="11771/69955" />
					<ITEM name="AAIA_ENGINE" value="8026" />
					<ITEM name="AAIA_LEGACY" value="1385276" />
					<ITEM name="AAIA_TRANSMISSION" value="742/2452" />
					<ITEM name="AAIA_VehicleID" value="11771/11771/11771/11771" />
					<ITEM name="AAIA_EngineConfigID" value="8026/8026/8026/8026" />
					<ITEM name="AAIA_TransmissionID" value="742/2452/742/2452" />
					<ITEM name="AAIA_BodyStyleConfigID" value="9/9/9/9" />
					<ITEM name="AAIA_BrakeConfigID" value="9/9/9/9" />
					<ITEM name="AAIA_DriveTypeID" value="8/8/5/5" />
					<ITEM name="AAIA_SpringTypeConfigID" value="1/1/1/1" />
					<ITEM name="Curb weight" value="3364" />
					<ITEM name="Gross vehicle weight rating" value="4520" />
					<ITEM name="Wheelbase" value="103.1" />
					<ITEM name="Overall length" value="173" />
					<ITEM name="Overall height" value="69.1" />
					<ITEM name="Overall width" value="70.1" />
					<ITEM name="Warranty whole vehicle Months" value="36" />
					<ITEM name="Warranty whole vehicle Miles" value="36000" />
					<ITEM name="Warranty powertrain Months" value="36" />
					<ITEM name="Warranty powertrain Miles" value="36000" />
					<ITEM name="Warranty anti-corrosion Months" value="60" />
					<ITEM name="Warranty anti-corrosion Miles" value="999999" />
					<ITEM name="Warranty roadside assistance Months" value="36" />
					<ITEM name="Warranty roadside assistance Miles" value="36000" />
					<ITEM name="MSRP" value="24000-26000" />
				</DECODED>
			</VIN>
		</VINPOWER>
	</REPORT>
</REPORTS>
```
