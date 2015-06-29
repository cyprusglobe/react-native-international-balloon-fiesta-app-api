# react-native-international-balloon-fiesta-app-api
Albuquerque International Balloon Fiesta App API

#### Current Route List

## Balloons Routes

```GET: /v2015/balloons?pilots_yes&balloons_no```

##### Get all balloons with pilot info

#### Result

```
{
  "balloon_name": "Balloon_Name",
  "balloon_size_unit": "cubic feet",
  "reg_num": "Balloon_Registration Number",
  "balloon_design_desc": "Balloon_Description",
  "pilot": [
  {
    "launch_sites": {
      "launch_thur_fri": "Launch_Site_Location",
      "launch_shapes": "Launch_Site_Location",
      "launch_9day": "Launch_Site_Location",
      "launch_balloon_glow": "Launch_Site_Location",
      "launch_rodeo": "Launch_Site_Location",
      "launch_night_magic": "Launch_Site_Location",
      "launch_twilight_twinkle": "Launch_Site_Location"
      },
      "city": "Pilot_City",
      "first_name": "Pilot_First_name",
      "last_name": "Pilot_Last_name",
      "state": "Pilot_State",
      "country": "Pilot_Country",
      "banner_number": Pilot_Banner_Number,
      "balloons": {},
        "id": Pilot_Id
      }
  ],
  "id": Balloon_Id,
  "shape_balloon": "Is_Balloon_Special_Shape",
  "balloon_size": Balloon_Cubic_Feet_Size
}
```

```GET: /v2015/balloons?pilots_no&balloons_no```

##### Get all balloons without pilot info

#### Result

```
{
"balloon_name": "Balloon_Name",
"balloon_size_unit": "cubic feet",
"reg_num": "Balloon_Registration Number",
"balloon_design_desc": "Balloon_Description",
"pilot": {},
"id": Balloon_Id,
"shape_balloon": "Is_Balloon_Special_Shape",
"balloon_size": Balloon_Cubic_Feet_Size
}
```

## Balloon Routes

```GET: /v2015/balloon/{balloon_id}?pilots_yes&balloons_no```

##### Get one balloon by id with pilot info

#### Result

```
{
  "balloon_name": "Balloon_Name",
  "balloon_size_unit": "cubic feet",
  "reg_num": "Balloon_Registration Number",
  "balloon_design_desc": "Balloon_Description",
  "pilot": {},
  "id": Balloon_Id,
  "shape_balloon": "Is_Balloon_Special_Shape",
  "balloon_size": Balloon_Cubic_Feet_Size
}
```

## Pilots Routes
```GET: /v2015/pilots?balloons_yes```

##### Get all pilots with balloon info

#### Result

```
{
  "launch_sites": {
      "launch_thur_fri": "Launch_Site_Location",
      "launch_shapes": "Launch_Site_Location",
      "launch_9day": "Launch_Site_Location",
      "launch_balloon_glow": "Launch_Site_Location",
      "launch_rodeo": "Launch_Site_Location",
      "launch_night_magic": "Launch_Site_Location",
      "launch_twilight_twinkle": "Launch_Site_Location"
    },
    "city": "Pilot_City",
    "first_name": "Pilot_First_name",
    "last_name": "Pilot_Last_name",
    "state": "Pilot_State",
    "country": "Pilot_Country",
    "banner_number": Pilot_Banner_Number,
    "balloons": [
      {
        "reg_num": "Balloon_Registration Number",
        "balloon_size_unit": "cubic feet",
        "shape_balloon": "Is_Balloon_Special_Shape",
        "balloon_name": "Balloon_Name"
        "balloon_design_desc": "Balloon_Description",
        "id": Balloon_Id,
        "balloon_size": Balloon_Cubic_Feet_Size
      }
    ],
    "id": Pilot_Id
}
```

```GET: /v2015/pilots?balloons_no```

##### Get all pilots without balloon info

#### Result

```
{
  "launch_sites": {
      "launch_thur_fri": "Launch_Site_Location",
      "launch_shapes": "Launch_Site_Location",
      "launch_9day": "Launch_Site_Location",
      "launch_balloon_glow": "Launch_Site_Location",
      "launch_rodeo": "Launch_Site_Location",
      "launch_night_magic": "Launch_Site_Location",
      "launch_twilight_twinkle": "Launch_Site_Location"
    },
    "city": "Pilot_City",
    "first_name": "Pilot_First_name",
    "last_name": "Pilot_Last_name",
    "state": "Pilot_State",
    "country": "Pilot_Country",
    "banner_number": Pilot_Banner_Number,
    "balloons": {}
    "id": Pilot_Id
}
```

## Pilot Routes
```GET: /v2015/pilot/{pilot_id}?balloons_yes```

##### Get one pilot by id with balloon info

#### Result

```
{
  "launch_sites": {
      "launch_thur_fri": "Launch_Site_Location",
      "launch_shapes": "Launch_Site_Location",
      "launch_9day": "Launch_Site_Location",
      "launch_balloon_glow": "Launch_Site_Location",
      "launch_rodeo": "Launch_Site_Location",
      "launch_night_magic": "Launch_Site_Location",
      "launch_twilight_twinkle": "Launch_Site_Location"
    },
    "city": "Pilot_City",
    "first_name": "Pilot_First_name",
    "last_name": "Pilot_Last_name",
    "state": "Pilot_State",
    "country": "Pilot_Country",
    "banner_number": Pilot_Banner_Number,
    "balloons": [
      {
        "reg_num": "Balloon_Registration Number",
        "balloon_size_unit": "cubic feet",
        "shape_balloon": "Is_Balloon_Special_Shape",
        "balloon_name": "Balloon_Name"
        "balloon_design_desc": "Balloon_Description",
        "id": Balloon_Id,
        "balloon_size": Balloon_Cubic_Feet_Size
      }
    ],
    "id": Pilot_Id
}
```

```GET: /v2015/pilot/{pilot_id}?balloons_no```

##### Get one pilot by id without balloon info

#### Result

```
{
  "launch_sites": {
      "launch_thur_fri": "Launch_Site_Location",
      "launch_shapes": "Launch_Site_Location",
      "launch_9day": "Launch_Site_Location",
      "launch_balloon_glow": "Launch_Site_Location",
      "launch_rodeo": "Launch_Site_Location",
      "launch_night_magic": "Launch_Site_Location",
      "launch_twilight_twinkle": "Launch_Site_Location"
    },
    "city": "Pilot_City",
    "first_name": "Pilot_First_name",
    "last_name": "Pilot_Last_name",
    "state": "Pilot_State",
    "country": "Pilot_Country",
    "banner_number": Pilot_Banner_Number,
    "balloons": {},
    "id": Pilot_Id
}
```

## Events Routes

```GET: /v2015/events```

##### Get all events

#### Result

```
{
  "date": "Event_Date",
  "events": [
    {
      "description": "Event_Description",
      "datetime": "2014-10-04 05:45:00"
    },
    {
      "description": "Event_Description",
      "datetime": "2014-10-04 06:30:00"
    },
    {
      "description": "Event_Description",
      "datetime": "2014-10-04 06:45:00"
    },
    {
      "description": "Event_Description",
      "datetime": "2014-10-04 07:00:00"
    },
    {
     "description": "Event_Description",
      "datetime": "2014-10-04 13:30:00"
    },
    {
      "description": "Event_Description",
      "datetime": "2014-10-04 14:00:00"
    },
    {
      "description": "Event_Description",
      "datetime": "2014-10-04 17:30:00"
    },
    {
      "description": "Event_Description",
      "datetime": "2014-10-04 17:45:00"
    },
    {
      "description": "Event_Description",
      "datetime": "2014-10-04 18:00:00"
    },
    {
      "description": "Event_Description",
      "datetime": "2014-10-04 20:00:00"
    }
  ]
}
```

## Location Routes

```GET: /v2015/locations```

##### Get all locations

#### Result

```
{
  "category": "Location_Category",
  "subtitle": "Location_Type",
  "title": "Location_Category",
  "lat": "Location_Latitude",
  "lon": "Location_Longitude",
  "type": "Location_Type",
  "name": "Location_Name",
  "description": "Location_Description"
}
```
