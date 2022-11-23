# Hi, this is MT Scripts mechanic script Installation Guide!!

# To start you just need to add your script to your resouces folder and follow the following instructions:
- Add images from mt-mechanic/images to qb-inventory/html/images;
- Add The following code to qb-inventory/html/app.js:

```
else if (itemData.name == "mechanic_paint_spray") {
            $(".item-info-title").html("<p>" + itemData.label + "</p>");
            $(".item-info-description").html("<p> <b> Color number: </b>" + itemData.info.paintNumber + "; <br> <b> Color type: </b>" + itemData.info.paintType +" <br> <b> Secound color type: " + itemData.info.paintType2 + " </b> </p> ");
        }
```
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
```
- Replace to qb-core/client/functions.lua where is QBCore.Functions.GetVehicleProperties():

```
function QBCore.Functions.GetVehicleProperties(vehicle)
    if DoesEntityExist(vehicle) then
        local pearlescentColor, wheelColor = GetVehicleExtraColours(vehicle)

        local colorPrimary, colorSecondary = GetVehicleColours(vehicle)
        if GetIsVehiclePrimaryColourCustom(vehicle) then
            local r, g, b = GetVehicleCustomPrimaryColour(vehicle)
            colorPrimary = {r, g, b}
        end

        if GetIsVehicleSecondaryColourCustom(vehicle) then
            local r, g, b = GetVehicleCustomSecondaryColour(vehicle)
            colorSecondary = {r, g, b}
        end

        local extras = {}
        for extraId = 0, 12 do
            if DoesExtraExist(vehicle, extraId) then
                local state = IsVehicleExtraTurnedOn(vehicle, extraId) == 1
                extras[tostring(extraId)] = state
            end
        end

        local modLivery = GetVehicleMod(vehicle, 48)
        if GetVehicleMod(vehicle, 48) == -1 and GetVehicleLivery(vehicle) ~= 0 then
            modLivery = GetVehicleLivery(vehicle)
        end

        local tireHealth = {}
        for i = 0, 3 do
            tireHealth[i] = GetVehicleWheelHealth(vehicle, i)
        end

        local tireBurstState = {}
        for i = 0, 5 do
           tireBurstState[i] = IsVehicleTyreBurst(vehicle, i, false)
        end

        local tireBurstCompletely = {}
        for i = 0, 5 do
            tireBurstCompletely[i] = IsVehicleTyreBurst(vehicle, i, true)
        end

        local windowStatus = {}
        for i = 0, 7 do
            windowStatus[i] = IsVehicleWindowIntact(vehicle, i) == 1
        end

        local doorStatus = {}
        for i = 0, 5 do
            doorStatus[i] = IsVehicleDoorDamaged(vehicle, i) == 1
        end

        return {
            model = GetEntityModel(vehicle),
            plate = QBCore.Functions.GetPlate(vehicle),
            plateIndex = GetVehicleNumberPlateTextIndex(vehicle),
            bodyHealth = QBCore.Shared.Round(GetVehicleBodyHealth(vehicle), 0.1),
            engineHealth = QBCore.Shared.Round(GetVehicleEngineHealth(vehicle), 0.1),
            tankHealth = QBCore.Shared.Round(GetVehiclePetrolTankHealth(vehicle), 0.1),
            fuelLevel = QBCore.Shared.Round(GetVehicleFuelLevel(vehicle), 0.1),
            dirtLevel = QBCore.Shared.Round(GetVehicleDirtLevel(vehicle), 0.1),
            oilLevel = QBCore.Shared.Round(GetVehicleOilLevel(vehicle), 0.1),
            color1 = colorPrimary,
            color2 = colorSecondary,
            pearlescentColor = pearlescentColor,
            dashboardColor = GetVehicleDashboardColour(vehicle),
            wheelColor = wheelColor,
            wheels = GetVehicleWheelType(vehicle),
            wheelSize = GetVehicleWheelSize(vehicle),
            wheelWidth = GetVehicleWheelWidth(vehicle),
            tireHealth = tireHealth,
            tireBurstState = tireBurstState,
            tireBurstCompletely = tireBurstCompletely,
            windowTint = GetVehicleWindowTint(vehicle),
            windowStatus = windowStatus,
            doorStatus = doorStatus,
            xenonColor = GetVehicleXenonLightsColour(vehicle),
            xenonColorRGB = table.pack(GetVehicleXenonLightsCustomColor(vehicle)),
            neonEnabled = {
                IsVehicleNeonLightEnabled(vehicle, 0),
                IsVehicleNeonLightEnabled(vehicle, 1),
                IsVehicleNeonLightEnabled(vehicle, 2),
                IsVehicleNeonLightEnabled(vehicle, 3)
            },
            neonColor = table.pack(GetVehicleNeonLightsColour(vehicle)),
            headlightColor = GetVehicleHeadlightsColour(vehicle),
            interiorColor = GetVehicleInteriorColour(vehicle),
            extras = extras,
            tyreSmokeColor = table.pack(GetVehicleTyreSmokeColor(vehicle)),
            modSpoilers = GetVehicleMod(vehicle, 0),
            modFrontBumper = GetVehicleMod(vehicle, 1),
            modRearBumper = GetVehicleMod(vehicle, 2),
            modSideSkirt = GetVehicleMod(vehicle, 3),
            modExhaust = GetVehicleMod(vehicle, 4),
            modFrame = GetVehicleMod(vehicle, 5),
            modGrille = GetVehicleMod(vehicle, 6),
            modHood = GetVehicleMod(vehicle, 7),
            modFender = GetVehicleMod(vehicle, 8),
            modRightFender = GetVehicleMod(vehicle, 9),
            modRoof = GetVehicleMod(vehicle, 10),
            modEngine = GetVehicleMod(vehicle, 11),
            modBrakes = GetVehicleMod(vehicle, 12),
            modTransmission = GetVehicleMod(vehicle, 13),
            modHorns = GetVehicleMod(vehicle, 14),
            modSuspension = GetVehicleMod(vehicle, 15),
            modArmor = GetVehicleMod(vehicle, 16),
            modKit17 = GetVehicleMod(vehicle, 17),
            modTurbo = IsToggleModOn(vehicle, 18),
            modNitrous = IsToggleModOn(vehicle, 17),
            modKit19 = GetVehicleMod(vehicle, 19),
            modSmokeEnabled = IsToggleModOn(vehicle, 20),
            modKit21 = GetVehicleMod(vehicle, 21),
            modXenon = IsToggleModOn(vehicle, 22),
            modFrontWheels = GetVehicleMod(vehicle, 23),
            modBackWheels = GetVehicleMod(vehicle, 24),
            modCustomTiresF = GetVehicleModVariation(vehicle, 23),
            modCustomTiresR = GetVehicleModVariation(vehicle, 24),
            modPlateHolder = GetVehicleMod(vehicle, 25),
            modVanityPlate = GetVehicleMod(vehicle, 26),
            modTrimA = GetVehicleMod(vehicle, 27),
            modOrnaments = GetVehicleMod(vehicle, 28),
            modDashboard = GetVehicleMod(vehicle, 29),
            modDial = GetVehicleMod(vehicle, 30),
            modDoorSpeaker = GetVehicleMod(vehicle, 31),
            modSeats = GetVehicleMod(vehicle, 32),
            modSteeringWheel = GetVehicleMod(vehicle, 33),
            modShifterLeavers = GetVehicleMod(vehicle, 34),
            modAPlate = GetVehicleMod(vehicle, 35),
            modSpeakers = GetVehicleMod(vehicle, 36),
            modTrunk = GetVehicleMod(vehicle, 37),
            modHydrolic = GetVehicleMod(vehicle, 38),
            modEngineBlock = GetVehicleMod(vehicle, 39),
            modAirFilter = GetVehicleMod(vehicle, 40),
            modStruts = GetVehicleMod(vehicle, 41),
            modArchCover = GetVehicleMod(vehicle, 42),
            modAerials = GetVehicleMod(vehicle, 43),
            modTrimB = GetVehicleMod(vehicle, 44),
            modTank = GetVehicleMod(vehicle, 45),
            modWindows = GetVehicleMod(vehicle, 46),
            modKit47 = GetVehicleMod(vehicle, 47),
            modLivery = modLivery,
            modKit49 = GetVehicleMod(vehicle, 49),
            liveryRoof = GetVehicleRoofLivery(vehicle),
            driftTyres = GetDriftTyresEnabled(vehicle),
        }
    else
        return
    end
end
```
- Replace to qb-core/client/functions.lua where is QBCore.Functions.SetVehicleProperties():

```
function QBCore.Functions.SetVehicleProperties(vehicle, props)
    if DoesEntityExist(vehicle) then
        if props.extras then
            for id, enabled in pairs(props.extras) do
                if enabled then
                    SetVehicleExtra(vehicle, tonumber(id), 0)
                else
                    SetVehicleExtra(vehicle, tonumber(id), 1)
                end
            end
        end

        local colorPrimary, colorSecondary = GetVehicleColours(vehicle)
        local pearlescentColor, wheelColor = GetVehicleExtraColours(vehicle)
        SetVehicleModKit(vehicle, 0)
        if props.plate then
            SetVehicleNumberPlateText(vehicle, props.plate)
        end
        if props.plateIndex then
            SetVehicleNumberPlateTextIndex(vehicle, props.plateIndex)
        end
        if props.bodyHealth then
            SetVehicleBodyHealth(vehicle, props.bodyHealth + 0.0)
        end
        if props.engineHealth then
            SetVehicleEngineHealth(vehicle, props.engineHealth + 0.0)
        end
        if props.tankHealth then
            SetVehiclePetrolTankHealth(vehicle, props.tankHealth)
        end
        if props.fuelLevel then
            SetVehicleFuelLevel(vehicle, props.fuelLevel + 0.0)
        end
        if props.dirtLevel then
            SetVehicleDirtLevel(vehicle, props.dirtLevel + 0.0)
        end
        if props.oilLevel then
            SetVehicleOilLevel(vehicle, props.oilLevel)
        end
        if props.color1 then
            if type(props.color1) == "number" then
                SetVehicleColours(vehicle, props.color1, colorSecondary)
            else
                SetVehicleCustomPrimaryColour(vehicle, props.color1[1], props.color1[2], props.color1[3])
            end
        end
        if props.color2 then
            if type(props.color2) == "number" then
                SetVehicleColours(vehicle, props.color1 or colorPrimary, props.color2)
            else
                SetVehicleCustomSecondaryColour(vehicle, props.color2[1], props.color2[2], props.color2[3])
            end
        end
        if props.pearlescentColor then
            SetVehicleExtraColours(vehicle, props.pearlescentColor, wheelColor)
        end
        if props.interiorColor then
            SetVehicleInteriorColor(vehicle, props.interiorColor)
        end
        if props.dashboardColor then
            SetVehicleDashboardColour(vehicle, props.dashboardColor)
        end
        if props.wheelColor then
            SetVehicleExtraColours(vehicle, props.pearlescentColor or pearlescentColor, props.wheelColor)
        end
        if props.wheels then
            SetVehicleWheelType(vehicle, props.wheels)
        end
        if props.tireHealth then
            for wheelIndex, health in pairs(props.tireHealth) do
                SetVehicleWheelHealth(vehicle, wheelIndex, health)
            end
        end
        if props.tireBurstState then
            for wheelIndex, burstState in pairs(props.tireBurstState) do
                if burstState then
                    SetVehicleTyreBurst(vehicle, tonumber(wheelIndex), false, 1000.0)
                end
            end
        end
        if props.tireBurstCompletely then
            for wheelIndex, burstState in pairs(props.tireBurstCompletely) do
                if burstState then
                    SetVehicleTyreBurst(vehicle, tonumber(wheelIndex), true, 1000.0)
                end
            end
        end
        if props.windowTint then
            SetVehicleWindowTint(vehicle, props.windowTint)
        end
        if props.windowStatus then
            for windowIndex, smashWindow in pairs(props.windowStatus) do
                if not smashWindow then SmashVehicleWindow(vehicle, windowIndex) end
            end
        end
        if props.doorStatus then
            for doorIndex, breakDoor in pairs(props.doorStatus) do
                if breakDoor then
                    SetVehicleDoorBroken(vehicle, tonumber(doorIndex), true)
                end
            end
        end
        if props.neonEnabled then
            SetVehicleNeonLightEnabled(vehicle, 0, props.neonEnabled[1])
            SetVehicleNeonLightEnabled(vehicle, 1, props.neonEnabled[2])
            SetVehicleNeonLightEnabled(vehicle, 2, props.neonEnabled[3])
            SetVehicleNeonLightEnabled(vehicle, 3, props.neonEnabled[4])
        end
        if props.neonColor then
            SetVehicleNeonLightsColour(vehicle, props.neonColor[1], props.neonColor[2], props.neonColor[3])
        end
        if props.headlightColor then
            SetVehicleHeadlightsColour(vehicle, props.headlightColor)
        end
        if props.interiorColor then
            SetVehicleInteriorColour(vehicle, props.interiorColor)
        end
        if props.wheelSize then
            SetVehicleWheelSize(vehicle, props.wheelSize)
        end
        if props.wheelWidth then
            SetVehicleWheelWidth(vehicle, props.wheelWidth)
        end
        if props.tyreSmokeColor then
            SetVehicleTyreSmokeColor(vehicle, props.tyreSmokeColor[1], props.tyreSmokeColor[2], props.tyreSmokeColor[3])
        end
        if props.modSpoilers then
            SetVehicleMod(vehicle, 0, props.modSpoilers, false)
        end
        if props.modFrontBumper then
            SetVehicleMod(vehicle, 1, props.modFrontBumper, false)
        end
        if props.modRearBumper then
            SetVehicleMod(vehicle, 2, props.modRearBumper, false)
        end
        if props.modSideSkirt then
            SetVehicleMod(vehicle, 3, props.modSideSkirt, false)
        end
        if props.modExhaust then
            SetVehicleMod(vehicle, 4, props.modExhaust, false)
        end
        if props.modFrame then
            SetVehicleMod(vehicle, 5, props.modFrame, false)
        end
        if props.modGrille then
            SetVehicleMod(vehicle, 6, props.modGrille, false)
        end
        if props.modHood then
            SetVehicleMod(vehicle, 7, props.modHood, false)
        end
        if props.modFender then
            SetVehicleMod(vehicle, 8, props.modFender, false)
        end
        if props.modRightFender then
            SetVehicleMod(vehicle, 9, props.modRightFender, false)
        end
        if props.modRoof then
            SetVehicleMod(vehicle, 10, props.modRoof, false)
        end
        if props.modEngine then
            SetVehicleMod(vehicle, 11, props.modEngine, false)
        end
        if props.modBrakes then
            SetVehicleMod(vehicle, 12, props.modBrakes, false)
        end
        if props.modTransmission then
            SetVehicleMod(vehicle, 13, props.modTransmission, false)
        end
        if props.modHorns then
            SetVehicleMod(vehicle, 14, props.modHorns, false)
        end
        if props.modSuspension then
            SetVehicleMod(vehicle, 15, props.modSuspension, false)
        end
        if props.modArmor then
            SetVehicleMod(vehicle, 16, props.modArmor, false)
        end
        if props.modKit17 then
            SetVehicleMod(vehicle, 17, props.modKit17, false)
        end
        if props.modTurbo then
            ToggleVehicleMod(vehicle, 18, props.modTurbo)
        end
        if props.modNitrous then
            ToggleVehicleMod(vehicle, 17, props.modNitrous)
        end
        if props.modKit19 then
            SetVehicleMod(vehicle, 19, props.modKit19, false)
        end
        if props.modSmokeEnabled then
            ToggleVehicleMod(vehicle, 20, props.modSmokeEnabled)
        end
        if props.modKit21 then
            SetVehicleMod(vehicle, 21, props.modKit21, false)
        end
        if props.modXenon then
            ToggleVehicleMod(vehicle, 22, props.modXenon)
        end
        if props.xenonColor then
            SetVehicleXenonLightsColor(vehicle, props.xenonColor)
        end
        if props.xenonColorRGB then
            SetVehicleXenonLightsCustomColor(vehicle, props.xenonColorRGB[2], props.xenonColorRGB[3], props.xenonColorRGB[4])
        end
        if props.modFrontWheels then
            SetVehicleMod(vehicle, 23, props.modFrontWheels, false)
        end
        if props.modBackWheels then
            SetVehicleMod(vehicle, 24, props.modBackWheels, false)
        end
        if props.modCustomTiresF then
            SetVehicleMod(vehicle, 23, props.modFrontWheels, props.modCustomTiresF)
        end
        if props.modCustomTiresR then
            SetVehicleMod(vehicle, 24, props.modBackWheels, props.modCustomTiresR)
        end
        if props.modPlateHolder then
            SetVehicleMod(vehicle, 25, props.modPlateHolder, false)
        end
        if props.modVanityPlate then
            SetVehicleMod(vehicle, 26, props.modVanityPlate, false)
        end
        if props.modTrimA then
            SetVehicleMod(vehicle, 27, props.modTrimA, false)
        end
        if props.modOrnaments then
            SetVehicleMod(vehicle, 28, props.modOrnaments, false)
        end
        if props.modDashboard then
            SetVehicleMod(vehicle, 29, props.modDashboard, false)
        end
        if props.modDial then
            SetVehicleMod(vehicle, 30, props.modDial, false)
        end
        if props.modDoorSpeaker then
            SetVehicleMod(vehicle, 31, props.modDoorSpeaker, false)
        end
        if props.modSeats then
            SetVehicleMod(vehicle, 32, props.modSeats, false)
        end
        if props.modSteeringWheel then
            SetVehicleMod(vehicle, 33, props.modSteeringWheel, false)
        end
        if props.modShifterLeavers then
            SetVehicleMod(vehicle, 34, props.modShifterLeavers, false)
        end
        if props.modAPlate then
            SetVehicleMod(vehicle, 35, props.modAPlate, false)
        end
        if props.modSpeakers then
            SetVehicleMod(vehicle, 36, props.modSpeakers, false)
        end
        if props.modTrunk then
            SetVehicleMod(vehicle, 37, props.modTrunk, false)
        end
        if props.modHydrolic then
            SetVehicleMod(vehicle, 38, props.modHydrolic, false)
        end
        if props.modEngineBlock then
            SetVehicleMod(vehicle, 39, props.modEngineBlock, false)
        end
        if props.modAirFilter then
            SetVehicleMod(vehicle, 40, props.modAirFilter, false)
        end
        if props.modStruts then
            SetVehicleMod(vehicle, 41, props.modStruts, false)
        end
        if props.modArchCover then
            SetVehicleMod(vehicle, 42, props.modArchCover, false)
        end
        if props.modAerials then
            SetVehicleMod(vehicle, 43, props.modAerials, false)
        end
        if props.modTrimB then
            SetVehicleMod(vehicle, 44, props.modTrimB, false)
        end
        if props.modTank then
            SetVehicleMod(vehicle, 45, props.modTank, false)
        end
        if props.modWindows then
            SetVehicleMod(vehicle, 46, props.modWindows, false)
        end
        if props.modKit47 then
            SetVehicleMod(vehicle, 47, props.modKit47, false)
        end
        if props.modLivery then
            SetVehicleMod(vehicle, 48, props.modLivery, false)
            SetVehicleLivery(vehicle, props.modLivery)
        end
        if props.modKit49 then
            SetVehicleMod(vehicle, 49, props.modKit49, false)
        end
        if props.liveryRoof then
            SetVehicleRoofLivery(vehicle, props.liveryRoof)
        end
        if props.driftTyres then
            SetDriftTyresEnabled(vehicle, true)
        end
    end
end
```
- Configure the script to your mlo's and perferences and enjoy!

# If need some help just join our discord and open an ticket, thanks for your purchase!