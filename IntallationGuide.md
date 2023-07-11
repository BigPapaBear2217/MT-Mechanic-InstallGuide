# Hi, this is MT Scripts mechanic script Installation Guide!!

# To start you just need to add your script to your resouces folder and follow the following instructions:
- Add images from mt-mechanic/images to qb-inventory/html/images;
- Add the following items to qb-core/shared/items.lua:

```
	-- mt-mechanic
	["mechanic_washing_kit"]     = {["name"] = "mechanic_washing_kit", 				    ["label"] = "Vehicle Washing Kit", 					["weight"] = 1000, 		["type"] = "item", 			["image"] = "mechanic_washing_kit.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "The best way to wash your vehicle!"},
	["mechanic_paint_spray"]     = {["name"] = "mechanic_paint_spray", 				    ["label"] = "Vehicle Paint Spray", 					["weight"] = 1000, 		["type"] = "item", 			["image"] = "mechanic_paint_spray.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "The best paint for you car!"},
	["mechanic_engine_lvl1"]     = {["name"] = "mechanic_engine_lvl1", 				    ["label"] = "Vehicle Engine LVL1", 					["weight"] = 50000, 		["type"] = "item", 			["image"] = "mechanic_engine_lvl1.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is a bad engine for your car!"},
	["mechanic_engine_lvl2"]     = {["name"] = "mechanic_engine_lvl2", 				    ["label"] = "Vehicle Engine LVL2", 					["weight"] = 50000, 		["type"] = "item", 			["image"] = "mechanic_engine_lvl2.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is an simple engine for your car!"},
	["mechanic_engine_lvl3"]     = {["name"] = "mechanic_engine_lvl3", 				    ["label"] = "Vehicle Engine LVL3", 					["weight"] = 50000, 		["type"] = "item", 			["image"] = "mechanic_engine_lvl3.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is an good engine for your car!"},
	["mechanic_engine_lvl4"]     = {["name"] = "mechanic_engine_lvl4", 				    ["label"] = "Vehicle Engine LVL4", 					["weight"] = 50000, 		["type"] = "item", 			["image"] = "mechanic_engine_lvl4.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is the best engine for your car!"},
	["mechanic_transmission_lvl1"]     = {["name"] = "mechanic_transmission_lvl1", 				    ["label"] = "Vehicle Transmission LVL1", 					["weight"] = 50000, 		["type"] = "item", 			["image"] = "mechanic_transmission_lvl1.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is a bad transmission for your car!"},
	["mechanic_transmission_lvl2"]     = {["name"] = "mechanic_transmission_lvl2", 				    ["label"] = "Vehicle Transmission LVL2", 					["weight"] = 50000, 		["type"] = "item", 			["image"] = "mechanic_transmission_lvl2.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is an simple transmission for your car!"},
	["mechanic_transmission_lvl3"]     = {["name"] = "mechanic_transmission_lvl3", 				    ["label"] = "Vehicle Transmission LVL3", 					["weight"] = 50000, 		["type"] = "item", 			["image"] = "mechanic_transmission_lvl3.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is an good transmission for your car!"},
	["mechanic_suspension_lvl1"]     = {["name"] = "mechanic_suspension_lvl1", 				    ["label"] = "Vehicle Suspension LVL1", 					["weight"] = 50000, 		["type"] = "item", 			["image"] = "mechanic_suspension_lvl1.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is a bad suspension for your car!"},
	["mechanic_suspension_lvl2"]     = {["name"] = "mechanic_suspension_lvl2", 				    ["label"] = "Vehicle Suspension LVL2", 					["weight"] = 50000, 		["type"] = "item", 			["image"] = "mechanic_suspension_lvl2.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is an simple suspension for your car!"},
	["mechanic_suspension_lvl3"]     = {["name"] = "mechanic_suspension_lvl3", 				    ["label"] = "Vehicle Suspension LVL3", 					["weight"] = 50000, 		["type"] = "item", 			["image"] = "mechanic_suspension_lvl3.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is a good suspension for your car!"},
	["mechanic_suspension_lvl4"]     = {["name"] = "mechanic_suspension_lvl4", 				    ["label"] = "Vehicle Suspension LVL4", 					["weight"] = 50000, 		["type"] = "item", 			["image"] = "mechanic_suspension_lvl4.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is the best suspension for your car!"},
	["mechanic_turbo"]     = {["name"] = "mechanic_turbo", 				    ["label"] = "Vehicle Turbo", 					["weight"] = 30000, 		["type"] = "item", 			["image"] = "mechanic_turbo.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is the best turbo for your car!"},
	["mechanic_armor"]     = {["name"] = "mechanic_armor", 				    ["label"] = "Vehicle Armor", 					["weight"] = 30000, 		["type"] = "item", 			["image"] = "mechanic_armor.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is the best way to keep your vehicle safe!"},
	["mechanic_tools"]     = {["name"] = "mechanic_tools", 				    ["label"] = "Tools", 					["weight"] = 2000, 		["type"] = "item", 			["image"] = "mechanic_tools.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "A good pack of tools to work in your car!"},
	["mechanic_toolbox"]     = {["name"] = "mechanic_toolbox", 				    ["label"] = "Tool Box", 					["weight"] = 5000, 		["type"] = "item", 			["image"] = "mechanic_toolbox.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "A good box to save your tools and things!"},
	["mechanic_neons_controller"]     = {["name"] = "mechanic_neons_controller", 				    ["label"] = "Vehicle Lights Controller", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_neons_controller.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "The best way to control your vehicle lights!"},
	["mechanic_brakes_lvl1"]     = {["name"] = "mechanic_brakes_lvl1", 				    ["label"] = "Vehicle Brakes LVL1", 					["weight"] = 40000, 		["type"] = "item", 			["image"] = "mechanic_brakes_lvl1.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is a bad brakes for your car!"},
	["mechanic_brakes_lvl2"]     = {["name"] = "mechanic_brakes_lvl2", 				    ["label"] = "Vehicle Brakes LVL2", 					["weight"] = 40000, 		["type"] = "item", 			["image"] = "mechanic_brakes_lvl2.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is a good brakes for your car!"},
	["mechanic_brakes_lvl3"]     = {["name"] = "mechanic_brakes_lvl3", 				    ["label"] = "Vehicle Brakes LVL3", 					["weight"] = 40000, 		["type"] = "item", 			["image"] = "mechanic_brakes_lvl3.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is the perfect brakes for your car!"},
	["mechanic_plate"]     = {["name"] = "mechanic_plate", 				    ["label"] = "Vehicle Plate", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_plate.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is the perfect plate for your car!"},
	["mechanic_window_tint"]     = {["name"] = "mechanic_window_tint", 				    ["label"] = "Vehicle Window Tint", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_window_tint.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is the best window tint for your car!"},
	["mechanic_livery"]     = {["name"] = "mechanic_livery", 				    ["label"] = "Vehicle Livery", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_livery.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "This is the best livery for your car!"},
	["mechanic_drift_tyres"]     = {["name"] = "mechanic_drift_tyres", 				    ["label"] = "Vehicle Drift Tyres", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_drift_tyres.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Want to make drift? Use this and see the magic!"},
	["mechanic_wheels"]     = {["name"] = "mechanic_wheels", 				    ["label"] = "Vehicle Wheels", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_wheels.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Why use default wheels?"},
	["mechanic_bumpers"]     = {["name"] = "mechanic_bumpers", 				    ["label"] = "Vehicle Bumper", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_bumpers.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Just make your vehicle more beatiful!"},
	["mechanic_bonnet"]     = {["name"] = "mechanic_bonnet", 				    ["label"] = "Vehicle Bonnet", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_bonnet.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Just make your vehicle more beatiful!"},
	["mechanic_skirt"]     = {["name"] = "mechanic_skirt", 				    ["label"] = "Vehicle Skirt", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_skirt.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Just make your vehicle more beatiful!"},
	["mechanic_spoiler"]     = {["name"] = "mechanic_spoiler", 				    ["label"] = "Vehicle Spoiler", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_spoiler.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Just make your vehicle more beatiful!"},
	["mechanic_horn"]     = {["name"] = "mechanic_horn", 				    ["label"] = "Vehicle Horn", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_horn.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Just put this on your vehicle and see the magic!"},
	["mechanic_grill"]     = {["name"] = "mechanic_grill", 				    ["label"] = "Vehicle Grill", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_grill.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "No it does not match to make meat xD"},
	["mechanic_nitrous"]     = {["name"] = "mechanic_nitrous", 				    ["label"] = "Vehicle Nitrous", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_nitrous.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "RACE! RACE! RACE! Take care of cops!"},
	["mechanic_exhaust"]     = {["name"] = "mechanic_exhaust", 				    ["label"] = "Vehicle Exhaust", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_exhaust.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "RATATATATA PA PA!"},
	["mechanic_nitrous_empty"]     = {["name"] = "mechanic_nitrous_empty", 				    ["label"] = "Vehicle Nitrous Empty", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_nitrous.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Ok... it seems that need something!"},
	["mechanic_mods_receipt"]     = {["name"] = "mechanic_mods_receipt", 				    ["label"] = "Vehicle Mods Receipt", 					["weight"] = 0, 		["type"] = "item", 			["image"] = "mechanic_mods_receipt.png", 		    ["unique"] = true, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Take this to any workshop!"},
	["mechanic_roof"]     = {["name"] = "mechanic_roof", 				    ["label"] = "Vehicle Roof", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_roof.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Roof Roof!"},
	["mechanic_extras"]     = {["name"] = "mechanic_extras", 				    ["label"] = "Vehicle Extras", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_extras.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Want to change some things at your vehicle? <br> Just use this!"},
	["mechanic_interior"]     = {["name"] = "mechanic_interior", 				    ["label"] = "Vehicle Interior", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_interior.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Need some confort? Use this shit at your car!"},
	["mechanic_exterior"]     = {["name"] = "mechanic_exterior", 				    ["label"] = "Vehicle Exterior Parts", 					["weight"] = 500, 		["type"] = "item", 			["image"] = "mechanic_exterior.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "IDK"},
	["mechanic_repair_kit"]     = {["name"] = "mechanic_repair_kit", 				    ["label"] = "Vehicle Repair Kit", 					["weight"] = 1000, 		["type"] = "item", 			["image"] = "repairkit.png", 		    ["unique"] = false, 	["useable"] = true, 	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "Just use this shit at your vehicle..."},
```

if you're using ox_inventory use this one:
```

	['mechanic_washing_kit'] = {
    	label = 'Car Wash Kit',
    	weight = 50,
		name = 'mechanic_washing_kit',
		description = "Car Washing Kit",
		useable = true,
    },

	['mechanic_paint_spray'] = {
    	label = 'Paint Spray',
    	weight = 50,
		name = 'mechanic_paint_spray',
		description = "Paint Spray",
		useable = true,
    },

	['mechanic_engine_lvl1'] = {
    	label = 'Engine LVL1',
    	weight = 100,
		name = 'mechanic_engine_lvl1',
		description = "Engine Level 1",
		useable = true,
    },

	['mechanic_engine_lvl2'] = {
    	label = 'Engine LVL2',
    	weight = 100,
		name = 'mechanic_engine_lvl2',
		description = "Engine Level 2",
		useable = true,
    },

	['mechanic_engine_lvl3'] = {
    	label = 'Engine LVL3',
    	weight = 100,
		name = 'mechanic_engine_lvl3',
		description = "Engine Level 3",
		useable = true,
    },
	
	['mechanic_engine_lvl4'] = {
    	label = 'Engine LVL4',
    	weight = 100,
		name = 'mechanic_engine_lvl4',
		description = "Engine Level 4",
		useable = true,
    },
		
	['mechanic_transmission_lvl1'] = {
    	label = 'Transmission LVL1',
    	weight = 100,
		name = 'mechanic_transmission_lvl1',
		description = "Transmission Level 1",
		useable = true,
    },
			
	['mechanic_transmission_lvl2'] = {
    	label = 'Transmission LVL2',
    	weight = 100,
		name = 'mechanic_transmission_lvl2',
		description = "Transmission Level 2",
		useable = true,
    },
				
	['mechanic_transmission_lvl3'] = {
    	label = 'Transmission LVL3',
    	weight = 100,
		name = 'mechanic_transmission_lvl3',
		description = "Transmission Level 3",
		useable = true,
    },
						
	['mechanic_suspension_lvl1'] = {
    	label = 'Suspension LVL1',
    	weight = 100,
		name = 'mechanic_suspension_lvl1',
		description = "Suspension Level 1",
		useable = true,
    },
							
	['mechanic_suspension_lvl2'] = {
    	label = 'Suspension LVL2',
    	weight = 100,
		name = 'mechanic_suspension_lvl1',
		description = "Suspension Level 2",
		useable = true,
    },
								
	['mechanic_suspension_lvl3'] = {
    	label = 'Suspension LVL3',
    	weight = 100,
		name = 'mechanic_suspension_lvl3',
		description = "Suspension Level 3",
		useable = true,
    },		

	['mechanic_suspension_lvl4'] = {
    	label = 'Suspension LVL4',
    	weight = 100,
		name = 'mechanic_suspension_lvl4',
		description = "Suspension Level 4",
		useable = true,
    },

	['mechanic_turbo'] = {
    	label = 'Turbo',
    	weight = 100,
		name = 'mechanic_turbo',
		description = "Turbo",
		useable = true,
    },

	['mechanic_armor'] = {
    	label = 'Armor',
    	weight = 100,
		name = 'mechanic_armor',
		description = "Armor",
		useable = true,
    },

	['mechanic_tools'] = {
    	label = 'Mechanic Tools',
    	weight = 100,
		name = 'mechanic_tools',
		description = "Mechanic Tools",
		useable = true,
    },

	['mechanic_toolbox'] = {
    	label = 'Portable Tool Box',
    	weight = 100,
		name = 'mechanic_toolbox',
		description = "Portable Tool Box",
		useable = true,
    },

	['mechanic_neons_controller'] = {
    	label = 'Neon Controller',
    	weight = 100,
		name = 'mechanic_neons_controller',
		description = "Neon Controller",
		useable = true,
    },

	['mechanic_brakes_lvl1'] = {
    	label = 'Brakes LVL1',
    	weight = 100,
		name = 'mechanic_brakes_lvl1',
		description = "Brakes Level 1",
		useable = true,
    },

	['mechanic_brakes_lvl2'] = {
    	label = 'Brakes LVL2',
    	weight = 100,
		name = 'mechanic_brakes_lvl2',
		description = "Brakes Level 2",
		useable = true,
    },

	['mechanic_brakes_lvl3'] = {
    	label = 'Brakes LVL3',
    	weight = 100,
		name = 'mechanic_brakes_lvl3',
		description = "Brakes Level 3",
		useable = true,
    },

	['mechanic_plate'] = {
    	label = 'License Plates',
    	weight = 100,
		name = 'mechanic_plate',
		description = "License Plates",
		useable = true,
    },

	['mechanic_window_tint'] = {
    	label = 'Window Tint',
    	weight = 100,
		name = 'mechanic_window_tint',
		description = "Windown Tint",
		useable = true,
    },

	['mechanic_livery'] = {
    	label = 'Stickers',
    	weight = 100,
		name = 'mechanic_livery',
		description = "Livery",
		useable = true,
    },

	['mechanic_drift_tyres'] = {
    	label = 'Drift Tires',
    	weight = 100,
		name = 'mechanic_drift_tyres',
		description = "Drift Tires",
		useable = true,
    },

	['mechanic_wheels'] = {
    	label = 'Wheels',
    	weight = 100,
		name = 'mechanic_wheels',
		description = "Wheels",
		useable = true,
    },

	['mechanic_bumpers'] = {
    	label = 'Bumpers',
    	weight = 100,
		name = 'mechanic_bumpers',
		description = "Bumpers",
		useable = true,
    },

	['mechanic_bonnet'] = {
    	label = 'Bonnet',
    	weight = 100,
		name = 'mechanic_bonnet',
		description = "Bonnet",
		useable = true,
    },

	['mechanic_skirt'] = {
    	label = 'Skirts',
    	weight = 100,
		name = 'mechanic_skirt',
		description = "Skirts",
		useable = true,
    },

	['mechanic_spoiler'] = {
    	label = 'Spoilers',
    	weight = 100,
		name = 'mechanic_spoiler',
		useable = true,
    },

	['mechanic_horn'] = {
    	label = 'Horn',
    	weight = 100,
		name = 'mechanic_horn',
		description = "Horn",
		useable = true,
    },

	['mechanic_grill'] = {
    	label = 'Grill',
    	weight = 100,
		name = 'mechanic_grill',
		description = "Grill",
		useable = true,
    },

	['mechanic_nitrous'] = {
    	label = 'Nitro',
    	weight = 100,
		name = 'mechanic_nitrous',
		description = "Nitro",
		useable = true,
    },

	['mechanic_exhaust'] = {
    	label = 'Exhaust',
    	weight = 100,
		name = 'mechanic_exhaust',
		description = "Exhaust",
		useable = true,
    },

	['mechanic_nitrous_empty'] = {
    	label = 'Empty Nitro',
    	weight = 100,
		name = 'mechanic_nitrous_empty',
		description = "Nitro Empty",
		useable = true,
    },
	
	['mechanic_mods_receipt'] = {
    	label = 'Receipt',
    	weight = 100,
		name = 'mechanic_mods_receipt',
		description = "List of Mods",
		useable = true,
    },

	['mechanic_roof'] = {
    	label = 'Roof',
    	weight = 100,
		name = 'mechanic_roof',
		description = "Roof",
		useable = true,
    },

	['mechanic_extras'] = {
    	label = 'Extras',
    	weight = 100,
		name = 'mechanic_extras',
		description = "Extras",
		useable = true,
    },

	['mechanic_interior'] = {
    	label = 'Interior',
    	weight = 100,
		name = 'mechanic_interior',
		description = "Interior",
		useable = true,
    },

	['mechanic_exterior'] = {
    	label = 'Exterior',
    	weight = 100,
		name = 'mechanic_exterior',
		description = "Exterior",
		useable = true,
    },

	['mechanic_repair_kit'] = {
    	label = 'Repair Kit',
    	weight = 100,
		name = 'mechanic_repair_kit',
		description = "Repair Kit",
		useable = true,
    },
```
- Configure the script to your mlo's and perferences and enjoy!

# If need some help just join our discord and open an ticket, thanks for your purchase!
