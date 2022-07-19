


    game.StarterGui:SetCore("SendNotification", {
        Title = "1tsJusthub";
        Text = "Loading!";
        Duration = "15";
        })

wait (0.8)        

    game.StarterGui:SetCore("SendNotification", {
        Title = "1tsJusthub";
        Text = "Loading Compleated";
        Duration = "15";
        })

wait (0.8)        

    game.StarterGui:SetCore("SendNotification", {
        Title = "1tsJustHub";
        Text = "Bully The Down Now";
        Duration = "15";
        })

wait (1.5)




local args = {
    [1] = "~1tsJustHub V2~",
    [2] = "All"
}

game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))

wait(0.4)


local args = {
    [1] = "~Credits 1tsJustgp~",
    [2] = "All"
}

game:GetService("ReplicatedStorage").DefaultChatSystemChatEvents.SayMessageRequest:FireServer(unpack(args))

wait(1.2)


    local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
    local Window = Library.CreateLib("1tsJustHub v2(DBZ FS)", "DarkTheme")
    
    --misc
    local Main = Window:NewTab("Misc")
    local MiscSection = Main:NewSection("Misc")





    MiscSection:NewButton("Noslow", "Za Za veloce veloce", function()
(getgenv()).noslow = true;

repeat
	wait();
until game:IsLoaded();
game.Players.LocalPlayer.PlayerGui:WaitForChild("HUD");
(game:GetService("RunService")).RenderStepped:Connect(function()
	for _, v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do
		if (getgenv()).noslow then
			if v.Name == "Action" or (v.Name == "Attacking") or 
            		(v.Name == "Using") or (v.Name == "hyper") or 
            		(v.Name == "Hyper") or (v.Name == "heavy") or 
            		(v.Name == "KiBlasted") or (v.Name == "Tele") or 
            		(v.Name == "tele") or (v.Name == "Killed") or 
            		(v.Name == "Slow") then
				v:Destroy();
			end;
			if game.Players.LocalPlayer.Character.Block.Value then
				game.Players.LocalPlayer.Character.Block.Value = false;
			end;
		end;
	end;
end);

    end)



		MiscSection:NewButton("God Mode (only earth)", "God modeMode rejoin for remove it", function()
		local Plr = game.Players.LocalPlayer
local GodModeBool = true

game:GetService("RunService").RenderStepped:connect(function()
if  GodModeBool  then
game.Workspace.Touchy.Part.CFrame = Plr.Character.HumanoidRootPart.CFrame + Vector3.new(0,0,1)
if Plr.PlayerGui:FindFirstChild("Popup") then
Plr.PlayerGui.Popup.Enabled = false
end
if not GodModeBool  then
return
end end end)
	end)


    MiscSection:NewButton("1tsJustCmds", "Use 1tsJustCmds", function()
        loadstring(game:HttpGet('https://raw.githubusercontent.com/gp1tsJust/1tsJustcmds-V1/main/README.md'))()
end)


        

        MiscSection:NewButton("Infiniti yield", "Infiniti yield", function()
            loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
    end)


    MiscSection:NewButton("Shaders", "Shaders", function()
        game.StarterGui:SetCore("SendNotification", {
            Title = "1tsJustHub";
            Text = "Shaders Loading";
            Duration = "15";
            })
            
            wait (1.5)
            
            local runDummyScript = function(f,scri)
            local oldenv = getfenv(f)
            local newenv = setmetatable({}, {
            __index = function(_, k)
            if k:lower() == 'script' then
            return scri
            else
            return oldenv[k]
            end
            end
            })
            setfenv(f, newenv)
            ypcall(function() f() end)
            end
            cors = {}
            mas = Instance.new("Model",game:GetService("Lighting")) 
            mas.Name = "CompiledModel"
            o2 = Instance.new("BloomEffect")
            o3 = Instance.new("BlurEffect")
            o4 = Instance.new("ColorCorrectionEffect")
            o5 = Instance.new("SunRaysEffect")
            o2.Parent = mas
            o2.Size = 56
            o2.Threshold = 0.98000001907349
            o3.Parent = mas
            o3.Size = 1.2199997901917
            o4.Parent = mas
            o4.Contrast = 0.52999997138977
            o4.Saturation = 0.098999999463558
            o4.Brightness = 0.070000000298023
            o5.Parent = mas
            o5.Intensity = 0.090000003576279
            mas.Parent = workspace
            mas:MakeJoints()
            local mas1 = mas:GetChildren()
            for i=1,#mas1 do
            mas1[i].Parent = game:GetService("Lighting") 
            ypcall(function() mas1[i]:MakeJoints() end)
            end
            mas:Destroy()
            for i=1,#cors do
            coroutine.resume(cors[i])
            end
            game:GetService("RunService").RenderStepped:Connect(function()
            game:GetService("Lighting").Ambient = Color3.new(0, 0, 0)
            game:GetService("Lighting").Brightness = 1
            game:GetService("Lighting").ColorShift_Bottom = Color3.new(0, 0, 0)
            game:GetService("Lighting").ColorShift_Top = Color3.new(0, 0, 0)
            game:GetService("Lighting").GlobalShadows = false
            game:GetService("Lighting").OutdoorAmbient = Color3.new(0.529412, 0.529412, 0.501961)
            game:GetService("Lighting").Outlines = true
            game:GetService("Lighting").GeographicLatitude = 41.733299255371
            game:GetService("Lighting").TimeOfDay = TimeOfDay
            game:GetService("Lighting").FogColor = Color3.new(0.75, 0.75, 0.75)
            game:GetService("Lighting").FogEnd = 7777777
            game:GetService("Lighting").FogStart = 7777777
            end)
    end)


	MiscSection:NewButton("2Exp_freeze", "2Exp_freeze", function()
		
--[[
AztupBrew(Fork of IronBrew2): obfuscation; Version 2.7.2
]]
return(function(NDR_h,NDR_a,NDR_l)local NDR_k=string.char;local NDR_e=string.sub;local NDR_p=table.concat;local NDR_o=math.ldexp;local NDR_r=getfenv or function()return _ENV end;local NDR_m=select;local NDR_g=unpack or table.unpack;local NDR_i=tonumber;local function NDR_n(NDR_h)local NDR_b,NDR_c,NDR_d="","",{}local NDR_g=256;local NDR_f={}for NDR_a=0,NDR_g-1 do NDR_f[NDR_a]=NDR_k(NDR_a)end;local NDR_a=1;local function NDR_j()local NDR_b=NDR_i(NDR_e(NDR_h,NDR_a,NDR_a),36)NDR_a=NDR_a+1;local NDR_c=NDR_i(NDR_e(NDR_h,NDR_a,NDR_a+NDR_b-1),36)NDR_a=NDR_a+NDR_b;return NDR_c end;NDR_b=NDR_k(NDR_j())NDR_d[1]=NDR_b;while NDR_a<#NDR_h do local NDR_a=NDR_j()if NDR_f[NDR_a]then NDR_c=NDR_f[NDR_a]else NDR_c=NDR_b..NDR_e(NDR_b,1,1)end;NDR_f[NDR_g]=NDR_b..NDR_e(NDR_c,1,1)NDR_d[#NDR_d+1],NDR_b,NDR_g=NDR_c,NDR_c,NDR_g+1 end;return table.concat(NDR_d)end;local NDR_j=NDR_n('22C22D27522C22827522D21221121G1Y21N22D22H27921Z27H27627922F27L27927523827M22D27427J27927427527N27T28027927R27Y28122J27P27I27H27427X22D22B23J22D27N27N28A27522728728228028H27521U27W27922E27922A27W22927921E21G21K21C22C22N2791I21C1X1621C2131Z21O21I29228V2751521L21G21829A21222C22M2791P21M21I21G21L29I29K29A22C22K2791M21P21G21321G21I1X29Y28X275112131W29F2791H21C2121X21321M21822D29P27527V27O22D23922I28727N21Z28428T28L28F2B223928L28X2B42872782B727P22B2AT28L29G27P28O2AA27P27X28Q2AS27P2AP27T2BI1Y21G21O1X22E25R25O2BX2BX26K22Y22C2BI28Z29122C22L2791S21229R21G21D21C21D22C2BF29W29L21329N2BO29R29T29V29J2CJ29Z2792CI29A1I1W21O22C27K22D122BS1X1J21M2132A221O21L2CF2B022D1T101H22E21A21T26Z1I25021B25T2C12DC1R1H1722D22528828R2AQ23A28N2B12B227U27P2DC2BA2792BI27S27N2BC2792A028I22923I2EC2802EF28727U2D02E521Y2B82BD2872BC2E627528V2ET22D2C72AY2B22A02B128O2EZ2AS2EZ2742942F22E02B121Z23G2792BO2AR2AO27P2BA28I22D2BL2812FN2F827T2DC29I2132C228Y2902922FP29629829A29C29E2CG2CT2CQ29M29O29Q29S29U2CU2FT2F12D12D621Q27B2A62922BI1P21O1Z2GK2791R2FW2FU2AB2AD2AF2752CD2AJ2AL2AN21X27I23E27S2752EW28T2EZ27N2E82BG2B328L2782F42FN2HG27Z2EQ2BB2HK28U22D2F62FN2B728I2C72B12742EW2A02EW2FP27S28B2DX2872DC2GT22D2BR2BT2772792GI27E2802862AQ2D02I12FJ2802FG2IH28R2EL2H52B22FN28M2842IN2842IU2FK27Q2I02752EB2872372362IY28T2EJ2IS28P2I22HJ2BF2I52C42FX29529729929B29D2GW22D2GC2CL2G92CO2GC2CS2752A22A42A62A82FT2BI2AC2AE2G42752AH2GZ2AM2FH2IF2I22AU2AW2HO2AZ2E128G2HM2752B62HE2KF28C2KJ2BF2IY2HB2812FM2I12792FP2I52I72BU2DI2DK2DM2DO2JC2GS2HT22D2C92CB2CD2CF2CH2G62CK2G82752CN2GB2LA2JR2JL2LA2CW2CY2D02D22BT2D52D721P2D92DB2792DE1H22C2DQ2DS2FL2DW2F52942742HJ2KA2E328S2792EW2KO2KE2J02I22J628R2FG2EN2EP2EW2ES2BE2KJ2EY2842GE2M62KB2I22HP2M52HC2M42E12FC2KS2M122D2HZ2II2BK2I228B2KT2FR21L2JX2FV2C52FY2JG2G12JJ2K12LI29X2LB2CM2GA2CP2NK2LH122GG2GI2G32GL2GN2GP2752GR2C52JY2GV2NI2GY2AK2K52H22AQ2H42IU2KJ2H82842KO28427N2EW2HF2BJ27I2HC2H628L2ML28728V2HP28B2HR2802L32EK2KJ2HX28L2HZ2J72OW28L');local NDR_a=(bit or bit32);local NDR_d=NDR_a and NDR_a.bxor or function(NDR_a,NDR_b)local NDR_c,NDR_d,NDR_e=1,0,10 while NDR_a>0 and NDR_b>0 do local NDR_e,NDR_f=NDR_a%2,NDR_b%2 if NDR_e~=NDR_f then NDR_d=NDR_d+NDR_c end NDR_a,NDR_b,NDR_c=(NDR_a-NDR_e)/2,(NDR_b-NDR_f)/2,NDR_c*2 end if NDR_a<NDR_b then NDR_a=NDR_b end while NDR_a>0 do local NDR_b=NDR_a%2 if NDR_b>0 then NDR_d=NDR_d+NDR_c end NDR_a,NDR_c=(NDR_a-NDR_b)/2,NDR_c*2 end return NDR_d end local function NDR_c(NDR_b,NDR_a,NDR_c)if NDR_c then local NDR_a=(NDR_b/2^(NDR_a-1))%2^((NDR_c-1)-(NDR_a-1)+1);return NDR_a-NDR_a%1;else local NDR_a=2^(NDR_a-1);return(NDR_b%(NDR_a+NDR_a)>=NDR_a)and 1 or 0;end;end;local NDR_a=1;local function NDR_b()local NDR_c,NDR_f,NDR_e,NDR_b=NDR_h(NDR_j,NDR_a,NDR_a+3);NDR_c=NDR_d(NDR_c,85)NDR_f=NDR_d(NDR_f,85)NDR_e=NDR_d(NDR_e,85)NDR_b=NDR_d(NDR_b,85)NDR_a=NDR_a+4;return(NDR_b*16777216)+(NDR_e*65536)+(NDR_f*256)+NDR_c;end;local function NDR_i()local NDR_b=NDR_d(NDR_h(NDR_j,NDR_a,NDR_a),85);NDR_a=NDR_a+1;return NDR_b;end;local function NDR_f()local NDR_b,NDR_c=NDR_h(NDR_j,NDR_a,NDR_a+2);NDR_b=NDR_d(NDR_b,85)NDR_c=NDR_d(NDR_c,85)NDR_a=NDR_a+2;return(NDR_c*256)+NDR_b;end;local function NDR_n()local NDR_d=NDR_b();local NDR_a=NDR_b();local NDR_e=1;local NDR_d=(NDR_c(NDR_a,1,20)*(2^32))+NDR_d;local NDR_b=NDR_c(NDR_a,21,31);local NDR_a=((-1)^NDR_c(NDR_a,32));if(NDR_b==0)then if(NDR_d==0)then return NDR_a*0;else NDR_b=1;NDR_e=0;end;elseif(NDR_b==2047)then return(NDR_d==0)and(NDR_a*(1/0))or(NDR_a*(0/0));end;return NDR_o(NDR_a,NDR_b-1023)*(NDR_e+(NDR_d/(2^52)));end;local NDR_o=NDR_b;local function NDR_q(NDR_b)local NDR_c;if(not NDR_b)then NDR_b=NDR_o();if(NDR_b==0)then return'';end;end;NDR_c=NDR_e(NDR_j,NDR_a,NDR_a+NDR_b-1);NDR_a=NDR_a+NDR_b;local NDR_b={}for NDR_a=1,#NDR_c do NDR_b[NDR_a]=NDR_k(NDR_d(NDR_h(NDR_e(NDR_c,NDR_a,NDR_a)),85))end return NDR_p(NDR_b);end;local NDR_a=NDR_b;local function NDR_o(...)return{...},NDR_m('#',...)end local function NDR_h()local NDR_k={};local NDR_j={};local NDR_a={};local NDR_l={[#{"1 + 1 = 111";{913;771;806;1};}]=NDR_j,[#{"1 + 1 = 111";"1 + 1 = 111";{388;597;52;718};}]=nil,[#{{356;848;894;622};"1 + 1 = 111";"1 + 1 = 111";"1 + 1 = 111";}]=NDR_a,[#{{99;244;668;95};}]=NDR_k,};local NDR_a=NDR_b()local NDR_e={}for NDR_c=1,NDR_a do local NDR_b=NDR_i();local NDR_a;if(NDR_b==0)then NDR_a=(NDR_i()~=0);elseif(NDR_b==3)then NDR_a=NDR_n();elseif(NDR_b==1)then NDR_a=NDR_q();end;NDR_e[NDR_c]=NDR_a;end;NDR_l[3]=NDR_i();for NDR_h=1,NDR_b()do local NDR_a=NDR_i();if(NDR_c(NDR_a,1,1)==0)then local NDR_d=NDR_c(NDR_a,2,3);local NDR_g=NDR_c(NDR_a,4,6);local NDR_a={NDR_f(),NDR_f(),nil,nil};if(NDR_d==0)then NDR_a[3]=NDR_f();NDR_a[4]=NDR_f();elseif(NDR_d==1)then NDR_a[3]=NDR_b();elseif(NDR_d==2)then NDR_a[3]=NDR_b()-(2^16)elseif(NDR_d==3)then NDR_a[3]=NDR_b()-(2^16)NDR_a[4]=NDR_f();end;if(NDR_c(NDR_g,1,1)==1)then NDR_a[2]=NDR_e[NDR_a[2]]end if(NDR_c(NDR_g,2,2)==1)then NDR_a[3]=NDR_e[NDR_a[3]]end if(NDR_c(NDR_g,3,3)==1)then NDR_a[4]=NDR_e[NDR_a[4]]end NDR_k[NDR_h]=NDR_a;end end;for NDR_a=1,NDR_b()do NDR_j[NDR_a-1]=NDR_h();end;return NDR_l;end;local function NDR_i(NDR_a,NDR_k,NDR_f)NDR_a=(NDR_a==true and NDR_h())or NDR_a;return(function(...)local NDR_d=NDR_a[1];local NDR_e=NDR_a[3];local NDR_j=NDR_a[2];local NDR_a=NDR_o local NDR_b=1;local NDR_a=-1;local NDR_o={};local NDR_n={...};local NDR_m=NDR_m('#',...)-1;local NDR_h={};local NDR_c={};for NDR_a=0,NDR_m do if(NDR_a>=NDR_e)then NDR_o[NDR_a-NDR_e]=NDR_n[NDR_a+1];else NDR_c[NDR_a]=NDR_n[NDR_a+#{"1 + 1 = 111";}];end;end;local NDR_a=NDR_m-NDR_e+1 local NDR_a;local NDR_e;while true do NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[1];if NDR_e<=23 then if NDR_e<=11 then if NDR_e<=5 then if NDR_e<=2 then if NDR_e<=0 then NDR_c[NDR_a[2]]=NDR_i(NDR_j[NDR_a[3]],nil,NDR_f);elseif NDR_e>1 then NDR_c[NDR_a[2]]=NDR_f[NDR_a[3]];else NDR_c[NDR_a[2]]=NDR_a[3];end;elseif NDR_e<=3 then local NDR_b=NDR_a[2]NDR_c[NDR_b]=NDR_c[NDR_b](NDR_g(NDR_c,NDR_b+1,NDR_a[3]))elseif NDR_e>4 then local NDR_a=NDR_a[2]NDR_c[NDR_a]=NDR_c[NDR_a](NDR_c[NDR_a+1])else NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];end;elseif NDR_e<=8 then if NDR_e<=6 then NDR_c[NDR_a[2]]=NDR_k[NDR_a[3]];elseif NDR_e==7 then if not NDR_c[NDR_a[2]]then NDR_b=NDR_b+1;else NDR_b=NDR_a[3];end;else if(NDR_c[NDR_a[2]]==NDR_a[4])then NDR_b=NDR_b+1;else NDR_b=NDR_a[3];end;end;elseif NDR_e<=9 then local NDR_b=NDR_a[2]NDR_c[NDR_b](NDR_g(NDR_c,NDR_b+1,NDR_a[3]))elseif NDR_e==10 then local NDR_g;local NDR_e;NDR_c[NDR_a[2]]=NDR_a[3];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2]NDR_c[NDR_e](NDR_c[NDR_e+1])NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_f[NDR_a[3]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2];NDR_g=NDR_c[NDR_a[3]];NDR_c[NDR_e+1]=NDR_g;NDR_c[NDR_e]=NDR_g[NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2]NDR_c[NDR_e]=NDR_c[NDR_e](NDR_c[NDR_e+1])NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];if NDR_c[NDR_a[2]]then NDR_b=NDR_b+1;else NDR_b=NDR_a[3];end;else if NDR_c[NDR_a[2]]then NDR_b=NDR_b+1;else NDR_b=NDR_a[3];end;end;elseif NDR_e<=17 then if NDR_e<=14 then if NDR_e<=12 then NDR_c[NDR_a[2]]=NDR_f[NDR_a[3]];elseif NDR_e>13 then NDR_c[NDR_a[2]]=(NDR_a[3]~=0);else NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_c[NDR_a[4]]];end;elseif NDR_e<=15 then local NDR_f;local NDR_e;NDR_e=NDR_a[2];NDR_f=NDR_c[NDR_a[3]];NDR_c[NDR_e+1]=NDR_f;NDR_c[NDR_e]=NDR_f[NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_a[3];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2]NDR_c[NDR_e]=NDR_c[NDR_e](NDR_g(NDR_c,NDR_e+1,NDR_a[3]))NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2];NDR_f=NDR_c[NDR_a[3]];NDR_c[NDR_e+1]=NDR_f;NDR_c[NDR_e]=NDR_f[NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2]NDR_c[NDR_e](NDR_c[NDR_e+1])NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_b=NDR_a[3];elseif NDR_e==16 then NDR_c[NDR_a[2]]();else if NDR_c[NDR_a[2]]then NDR_b=NDR_b+1;else NDR_b=NDR_a[3];end;end;elseif NDR_e<=20 then if NDR_e<=18 then NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];elseif NDR_e>19 then local NDR_f;local NDR_e;NDR_e=NDR_a[2];NDR_f=NDR_c[NDR_a[3]];NDR_c[NDR_e+1]=NDR_f;NDR_c[NDR_e]=NDR_f[NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_a[3];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2]NDR_c[NDR_e]=NDR_c[NDR_e](NDR_g(NDR_c,NDR_e+1,NDR_a[3]))NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2];NDR_f=NDR_c[NDR_a[3]];NDR_c[NDR_e+1]=NDR_f;NDR_c[NDR_e]=NDR_f[NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2]NDR_c[NDR_e](NDR_c[NDR_e+1])NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_b=NDR_a[3];else local NDR_h;local NDR_e;NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2];NDR_h=NDR_c[NDR_a[3]];NDR_c[NDR_e+1]=NDR_h;NDR_c[NDR_e]=NDR_h[NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_a[3];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2]NDR_c[NDR_e](NDR_g(NDR_c,NDR_e+1,NDR_a[3]))NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_f[NDR_a[3]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_a[3];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2]NDR_c[NDR_e](NDR_c[NDR_e+1])end;elseif NDR_e<=21 then NDR_c[NDR_a[2]]=NDR_k[NDR_a[3]];elseif NDR_e==22 then NDR_b=NDR_a[3];else do return end;end;elseif NDR_e<=35 then if NDR_e<=29 then if NDR_e<=26 then if NDR_e<=24 then NDR_c[NDR_a[2]]=NDR_i(NDR_j[NDR_a[3]],nil,NDR_f);elseif NDR_e==25 then NDR_c[NDR_a[2]]=NDR_a[3];else NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]];end;elseif NDR_e<=27 then NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_c[NDR_a[4]]];elseif NDR_e==28 then do return end;else local NDR_j=NDR_j[NDR_a[3]];local NDR_g;local NDR_e={};NDR_g=NDR_l({},{__index=function(NDR_b,NDR_a)local NDR_a=NDR_e[NDR_a];return NDR_a[1][NDR_a[2]];end,__newindex=function(NDR_c,NDR_a,NDR_b)local NDR_a=NDR_e[NDR_a]NDR_a[1][NDR_a[2]]=NDR_b;end;});for NDR_f=1,NDR_a[4]do NDR_b=NDR_b+1;local NDR_a=NDR_d[NDR_b];if NDR_a[1]==26 then NDR_e[NDR_f-1]={NDR_c,NDR_a[3]};else NDR_e[NDR_f-1]={NDR_k,NDR_a[3]};end;NDR_h[#NDR_h+1]=NDR_e;end;NDR_c[NDR_a[2]]=NDR_i(NDR_j,NDR_g,NDR_f);end;elseif NDR_e<=32 then if NDR_e<=30 then NDR_f[NDR_a[3]]=NDR_c[NDR_a[2]];elseif NDR_e==31 then NDR_c[NDR_a[2]]=(NDR_a[3]~=0);else NDR_c[NDR_a[2]]();end;elseif NDR_e<=33 then local NDR_a=NDR_a[2]NDR_c[NDR_a](NDR_c[NDR_a+1])elseif NDR_e==34 then local NDR_a=NDR_a[2]NDR_c[NDR_a](NDR_c[NDR_a+1])else local NDR_g;local NDR_e;NDR_c[NDR_a[2]]=NDR_a[3];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2]NDR_c[NDR_e](NDR_c[NDR_e+1])NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_f[NDR_a[3]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2];NDR_g=NDR_c[NDR_a[3]];NDR_c[NDR_e+1]=NDR_g;NDR_c[NDR_e]=NDR_g[NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2]NDR_c[NDR_e]=NDR_c[NDR_e](NDR_c[NDR_e+1])NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];if not NDR_c[NDR_a[2]]then NDR_b=NDR_b+1;else NDR_b=NDR_a[3];end;end;elseif NDR_e<=41 then if NDR_e<=38 then if NDR_e<=36 then local NDR_d=NDR_a[2];local NDR_b=NDR_c[NDR_a[3]];NDR_c[NDR_d+1]=NDR_b;NDR_c[NDR_d]=NDR_b[NDR_a[4]];elseif NDR_e>37 then local NDR_b=NDR_a[2];local NDR_d=NDR_c[NDR_a[3]];NDR_c[NDR_b+1]=NDR_d;NDR_c[NDR_b]=NDR_d[NDR_a[4]];else if not NDR_c[NDR_a[2]]then NDR_b=NDR_b+1;else NDR_b=NDR_a[3];end;end;elseif NDR_e<=39 then if(NDR_c[NDR_a[2]]==NDR_a[4])then NDR_b=NDR_b+1;else NDR_b=NDR_a[3];end;elseif NDR_e>40 then NDR_f[NDR_a[3]]=NDR_c[NDR_a[2]];else local NDR_h;local NDR_e;NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2];NDR_h=NDR_c[NDR_a[3]];NDR_c[NDR_e+1]=NDR_h;NDR_c[NDR_e]=NDR_h[NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_a[3];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2]NDR_c[NDR_e](NDR_g(NDR_c,NDR_e+1,NDR_a[3]))NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_f[NDR_a[3]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_a[3];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2]NDR_c[NDR_e](NDR_c[NDR_e+1])end;elseif NDR_e<=44 then if NDR_e<=42 then local NDR_j=NDR_j[NDR_a[3]];local NDR_g;local NDR_e={};NDR_g=NDR_l({},{__index=function(NDR_b,NDR_a)local NDR_a=NDR_e[NDR_a];return NDR_a[1][NDR_a[2]];end,__newindex=function(NDR_c,NDR_a,NDR_b)local NDR_a=NDR_e[NDR_a]NDR_a[1][NDR_a[2]]=NDR_b;end;});for NDR_f=1,NDR_a[4]do NDR_b=NDR_b+1;local NDR_a=NDR_d[NDR_b];if NDR_a[1]==26 then NDR_e[NDR_f-1]={NDR_c,NDR_a[3]};else NDR_e[NDR_f-1]={NDR_k,NDR_a[3]};end;NDR_h[#NDR_h+1]=NDR_e;end;NDR_c[NDR_a[2]]=NDR_i(NDR_j,NDR_g,NDR_f);elseif NDR_e==43 then NDR_b=NDR_a[3];else local NDR_a=NDR_a[2]NDR_c[NDR_a]=NDR_c[NDR_a](NDR_c[NDR_a+1])end;elseif NDR_e<=46 then if NDR_e==45 then local NDR_h;local NDR_e;NDR_c[NDR_a[2]]=NDR_f[NDR_a[3]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2];NDR_h=NDR_c[NDR_a[3]];NDR_c[NDR_e+1]=NDR_h;NDR_c[NDR_e]=NDR_h[NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_a[3];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2]NDR_c[NDR_e]=NDR_c[NDR_e](NDR_g(NDR_c,NDR_e+1,NDR_a[3]))NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_f[NDR_a[3]]=NDR_c[NDR_a[2]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_f[NDR_a[3]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_f[NDR_a[3]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_c[NDR_a[4]]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2];NDR_h=NDR_c[NDR_a[3]];NDR_c[NDR_e+1]=NDR_h;NDR_c[NDR_e]=NDR_h[NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2]NDR_c[NDR_e](NDR_c[NDR_e+1])NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];do return end;else local NDR_b=NDR_a[2]NDR_c[NDR_b]=NDR_c[NDR_b](NDR_g(NDR_c,NDR_b+1,NDR_a[3]))end;elseif NDR_e==47 then local NDR_h;local NDR_e;NDR_c[NDR_a[2]]=NDR_f[NDR_a[3]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2];NDR_h=NDR_c[NDR_a[3]];NDR_c[NDR_e+1]=NDR_h;NDR_c[NDR_e]=NDR_h[NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_a[3];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2]NDR_c[NDR_e]=NDR_c[NDR_e](NDR_g(NDR_c,NDR_e+1,NDR_a[3]))NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_f[NDR_a[3]]=NDR_c[NDR_a[2]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_f[NDR_a[3]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_f[NDR_a[3]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_c[NDR_a[4]]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_c[NDR_a[2]]=NDR_c[NDR_a[3]][NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2];NDR_h=NDR_c[NDR_a[3]];NDR_c[NDR_e+1]=NDR_h;NDR_c[NDR_e]=NDR_h[NDR_a[4]];NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];NDR_e=NDR_a[2]NDR_c[NDR_e](NDR_c[NDR_e+1])NDR_b=NDR_b+1;NDR_a=NDR_d[NDR_b];do return end;else local NDR_b=NDR_a[2]NDR_c[NDR_b](NDR_g(NDR_c,NDR_b+1,NDR_a[3]))end;NDR_b=NDR_b+1;end;end);end;return NDR_i(true,{},NDR_r())();end)(string.byte,table.insert,setmetatable);

	end)


    	--Bully



        local Main = Window:NewTab("Bully")
        local BullySection = Main:NewSection("Bully Mode")
    
    
        BullySection:NewButton("Dragon Trow Glich", "Dragon Trow Glich", function()
            local player = game.Players.LocalPlayer
            local Character = player.character
            while wait(0.3) do
                player.Backpack:WaitForChild("Dragon Throw")
                player.Backpack["Dragon Throw"].Activator:WaitForChild("Flip")
                wait()
                if (player.Backpack:FindFirstChild("Dragon Throw")) then
                    repeat
                        wait()
                    until player.Character:FindFirstChild("Dragon Throw")
        
                    repeat
                        wait()
                    until Character.Ki.Value < Character.Ki.MaxValue
                end
                repeat
                    wait()
                    Character["Dragon Throw"].Activator:FindFirstChild("Flip"):Destroy()
                until not Character["Dragon Throw"].Activator:FindFirstChild("Flip")
            end
        end)
    
        BullySection:NewButton("Dragon Crush Glich", "Dragon Crush Glich", function()
            local player = game.Players.LocalPlayer
            local Character = player.character
            while wait(0.3) do
                player.Backpack:WaitForChild("Dragon Crush")
                player.Backpack["Dragon Crush"].Activator:WaitForChild("Flip")
                wait()
                if (player.Backpack:FindFirstChild("Dragon Crush")) then
                    repeat
                        wait()
                    until player.Character:FindFirstChild("Dragon Crush")
        
                    repeat
                        wait()
                    until Character.Ki.Value < Character.Ki.MaxValue
                end
                repeat
                    wait()
                    Character["Dragon Crush"].Activator:FindFirstChild("Flip"):Destroy()
                until not Character["Dragon Crush"].Activator:FindFirstChild("Flip")
            end
        
        end)


        BullySection:NewButton("Bone Crush Glich", "Pressing V while bone crush equipped will", function()
            wait()
game:GetService("StarterGui"):SetCore("SendNotification", {Title = "1tsJustHub", Text = "After glich Hard Reset For Moves  ",})

local mouse = game.Players.LocalPlayer:GetMouse()
mouse.KeyDown:connect(function(key)
    if key == "v" then
        local lplr = game.Players.LocalPlayer
        lplr.Character["Bone Crush"].Activator.Crash:Destroy()
    end
end)

        end)
    
    
    
        BullySection:NewToggle("Anchor", "Anchor Charapter", function(state)
            if state then
                game.Players.LocalPlayer.Character.HumanoidRootPart.Anchored = true 
            else
                game.Players.LocalPlayer.Character.HumanoidRootPart.Anchored = false 
            end
        end)
    
        BullySection:NewKeybind("Fast God", "Fast God Form", Enum.KeyCode.U, function()
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "decrease"},[2] = true}))
            game:GetService("ReplicatedStorage").ResetChar:FireServer()
            wait(0.4)
            local args = {
                [1] = "h"
            }
            
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Transform:FireServer(unpack(args))
            wait(0.4)
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            game:GetService("Players").LocalPlayer.Backpack.ServerTraits.Input:FireServer(unpack( {[1] = {[1] = "increase"},[2] = true}))
            
            getgenv().showstats = true
            getgenv().Zenni = true
            getgenv().resettop = true 
            getgenv().RespawnLowKi = true
            getgenv().movespam = true;
            getgenv().noslow = true;
            getgenv().Spambans = true;
            local plr = game.Players.LocalPlayer 
        end)
        
    
    
    
        BullySection:NewButton("Melee Spam", "Press V to spam", function()
            Move1 = "Anger Rush"
    Move2 = "Sweep Kick"
    Move3 = "Trash???"
    Move4 = "Neo Wolf Fang Fist"
    Move5 = "Wolf Fang Fist"
    Move6 = "TS Molotov"
    Move7 = "Trash?"
    Move8 = "Deadly Dance"
    Move9 = "God Slicer"
    --
    MSKey = "v" -- Change the key inside the quotations to whatever key you want to use to toggle your movespam.
    --
    _cMhlNnFWdeO1FLGW, Protected_by_MoonSecV2, Discord = 'discord.gg/gQEH2uZxUk'
    ,nil,nil;(function() _msec=(function(_,_l,__)local __l__l=_l["㒞㒙㒡㒣㒞㒙㒢㒞㒡㒗㒤㒥㒝㒞"];local _ll__l=__[_[(-#{'nil';(function()return{','}end)(),1,'}',(function()return#{('pFFFbm'):find("\70")}>0 and 1 or 0 end)}+645)]][_["㒤㒥㒞㒛㒚㒚㒥㒙㒚㒥"]];local __ll=(0x46-66)/(0x49+(-#[[im dying]]+((-8+-0x2c)-11)))local _lll=((0xa1+(-0xbc1/51))+-0x64)-(38-0x25)local ___lll=__[_[(0x1bb-265)]][_["㒘㒚㒢㒘㒛㒗㒗㒛㒛"]];local __l__=(((0x171+((-167+0x32)+-#[[Fuck]]))-169)+-0x4e)+(44+-0x2a)local _l_ll=__[_[(596+-#{",",85;'}';'nil';(function()return{','}end)(),150,'}'})]][_["㒛㒙㒗㒛㒝㒠㒞㒢㒞㒛㒢㒠㒡㒜"]]local __l=((0x12a1/251)+-#'free nitro real?!')-((0x7d+(-25+((-78+0xb)+-#[[cock and ball]])))+-#[[happy birdday wally]])local ____l=((((4080+-#{(function()return{','}end)();'nil',(function()return#{('fpPfll'):find("\80")}>0 and 1 or 0 end)})/27)+-#"deobfuscation in progress")+-0x7a)local _lll_=((((0x22d-(313+-#{(function()return{','}end)(),30;{};'nil',{},1;","}))+-#'This code was obfuscated using PSU, which stands for Penis Sucking Utilities')-106)+-#'guys i am epic hackerman i just converted a script to string.byte')local _l___=(-#[[am gay]]+(-0x7d+(0xea+((-#'How to dump moonsec'+(-0x343f7a/234))/0x94))))local __llll=((-#{'}';",",133;",";",",(function()return#{('BHbkpP'):find("\98")}>0 and 1 or 0 end)}+69)+-0x3b)local _l_l_=((-104-((-0xd12+-42)/0x9a))+86)local __ll_=(((-0x5b+((601+-0x59)-0x117))+-#[[_Ben is godly]])-125)local __lll=(0xc8/((325+-#{{},79;79;(function()return{','}end)(),25;79})-219))local ___l=(6+-#{1,",";(function()return{','}end)(),1})local _l__l=(63+(-#"bit.bdiv(0,0)"+((89-(249-((-94+0x122)+-#[[obfuscator tooooo gooood]])))-60)))local _ll_=(-#'are you maybe is the or the maybe is the or the maybe hm'+(((-0x5348/(513-(0x167+-51)))-3)+165))local ___ll=((-59+(0x12e+((-124+0x2c)+-#'FREE LUA OBFUSCATOR DOWNLOAD REAL NO FAKE 2024')))+-115)local __l_=(432/((54145/(58310/(-#[[string]]+(0x346c/55))))+-#'troll'))local __l_l=((-90+(147+-#{'}',{},1;(function()return{','}end)();104,{};(function()return#{('BFmHoP'):find("\109")}>0 and 1 or 0 end)}))+-#'psst constant table just below this meme string')local _l_l=((((-0xd26d+26905)/0x7e)+0x57)+130)local ____=(-#{",";{};(function()return{','}end)()}+6)local _l__=((100+-#{'nil',",";",",1,1})+-0x5c)local _llll=(9+-#{(function()return{','}end)(),73;95,95,73;","})local _ll_l=((144-((1789+-#{",",60;168;60})/15))+-#"what the fuck is sleep")local __ll_l=_[(1394+-#{'}',{};'}','nil';1,86})];local _l_l_l=__[_[(185+-#{(function()return{','}end)(),'}';{};131,1,54,'nil'})]][_["㒘㒥㒛㒥㒛㒘㒝㒛"]];local _lll_l=__[(function(_)return type(_):sub(1,1)..'\101\116'end)('㒝㒣㒦㒠㒘㒤㒘㒠')..'\109\101'..('\116\97'or'㒞㒘㒘㒝㒦㒙㒡㒞').._[((-0x39-28)+0x2a2)]];local __l_ll=__[_[(1245-0x290)]][_["㒟㒛㒙㒙㒢㒜㒦㒛㒛㒚"]];local _lllll=(186/0x5d)-(50-(-#'this file has been secured with a wall the size of your mother'+((0x2102/26)-215)))local _____=(-0x2e+((193+(-119+0x23))+-#[[psu got dumped so hard their entire source code came out rofl]]))-(-86+0x58)local _l__ll=__[_[(184+-#{'}',",";'}';{};'}';{}})]][_["㒝㒡㒞㒤㒜㒤㒚㒜㒝㒡㒡㒥㒞㒥㒙㒤"]];local _l=function(_l,_)return _l.._ end local _l_lll=(0x3f-59)*(57+((-0x31-((-0x35+68)+-#[[Why are you reading this]]))+-#"constant dumB"))local ____ll=__[_["㒟㒡㒗㒣㒤㒞㒢㒞㒠㒡㒘"]];local ___=(0x28/20)*(25216/((9547014/0xf6)/0xc5))local _ll_ll=((-0x55+104533)/0x66)*((128-((-204+0x56)+0xcb))+-#"oh oh i will hack you =opens dev console=")local ___l_l=(0x90-(-#[[is it me or everyones feeling like ghostpinging <@!519139355118534656> ?]]+(-84+(0x23a-322))))local _ll__=(-#[[are you maybe is the or the maybe is the or the maybe hm]]+(((-109+0x16)+253)-0x6c))*(-#[[i dont care that this was enchanted with uncrackable V]]+(134-0x4e))local ___l_=__[_["㒦㒝㒝㒦㒘㒚㒣㒞㒡"]]or __[_[((1284-0x2a6)+-#[[while true do end]])]][_["㒦㒝㒝㒦㒘㒚㒣㒞㒡"]];local _l_=(((2489-0x514)-0x27f)-294)local _=__[_["㒟㒛㒚㒙㒢㒦㒗㒢㒞㒥㒥㒦"]];local __l_ll=(function(_l_)local ___,__=3,0x10 local _l={j={},v={}}local _ll=-__l local _=__+_lll while true do _l[_l_:sub(_,(function()_=___+_ return _-_lll end)())]=(function()_ll=_ll+__l return _ll end)()if _ll==(_l_lll-__l)then _ll=""__=_lllll break end end local _ll=#_l_ while _<_ll+_lll do _l.v[__]=_l_:sub(_,(function()_=___+_ return _-_lll end)())__=__+__l if __%__ll==_lllll then __=_____ __l_ll(_l.j,(_l__ll((_l[_l.v[_____]]*_l_lll)+_l[_l.v[__l]])))end end return _l_ll(_l.j)end)("..:::MoonSec::..㒗㒘㒙㒚㒛㒜㒝㒞㒟㒠㒡㒢㒣㒤㒥㒦㒦㒣㒛㒞㒦㒞㒡㒞㒙㒦㒘㒗㒢㒞㒝㒞㒘㒞㒗㒡㒤㒦㒟㒟㒛㒠㒥㒟㒠㒡㒜㒢㒦㒣㒢㒠㒦㒟㒢㒗㒜㒞㒗㒞㒢㒞㒤㒥㒟㒝㒚㒠㒥㒙㒠㒡㒛㒞㒥㒟㒠㒡㒛㒣㒠㒟㒜㒘㒦㒞㒡㒞㒜㒞㒛㒤㒙㒗㒤㒠㒞㒣㒘㒡㒤㒣㒠㒠㒛㒤㒥㒣㒡㒠㒥㒟㒡㒗㒛㒞㒦㒞㒡㒞㒡㒥㒝㒟㒙㒚㒤㒙㒟㒡㒚㒞㒤㒣㒟㒣㒚㒢㒢㒚㒛㒚㒥㒞㒠㒞㒛㒞㒛㒢㒘㒠㒣㒗㒝㒥㒘㒥㒣㒣㒟㒠㒗㒣㒥㒤㒟㒣㒛㒜㒦㒢㒢㒠㒦㒗㒠㒞㒛㒞㒦㒞㒦㒞㒣㒚㒝㒟㒚㒗㒣㒣㒟㒠㒗㒥㒥㒣㒠㒗㒜㒠㒟㒣㒚㒞㒥㒞㒠㒞㒟㒤㒝㒝㒘㒠㒢㒡㒝㒣㒚㒠㒝㒣㒘㒞㒣㒞㒞㒞㒝㒡㒚㒦㒥㒣㒡㒡㒜㒢㒘㒠㒛㒠㒦㒞㒡㒞㒜㒞㒝㒝㒦㒥㒥㒠㒙㒘㒣㒞㒞㒞㒙㒞㒘㒥㒥㒣㒡㒢㒚㒡㒦㒣㒢㒠㒝㒤㒘㒗㒢㒡㒝㒣㒚㒠㒝㒤㒘㒞㒣㒞㒞㒞㒞㒞㒛㒚㒥㒟㒢㒗㒛㒣㒗㒠㒛㒟㒦㒦㒡㒞㒜㒞㒗㒞㒦㒦㒤㒢㒟㒢㒚㒞㒣㒞㒠㒝㒛㒡㒦㒢㒗㒦㒦㒘㒠㒞㒛㒞㒦㒞㒗㒝㒢㒝㒞㒡㒘㒣㒣㒡㒟㒣㒚㒠㒤㒣㒟㒣㒛㒟㒚㒛㒚㒡㒥㒞㒠㒞㒛㒞㒛㒚㒗㒣㒢㒥㒗㒟㒢㒣㒝㒞㒘㒞㒣㒞㒢㒡㒠㒚㒛㒝㒦㒥㒡㒜㒘㒚㒡㒗㒛㒞㒦㒞㒡㒞㒢㒥㒝㒟㒙㒛㒣㒣㒟㒡㒙㒣㒥㒜㒠㒡㒚㒣㒤㒥㒛㒙㒥㒞㒠㒞㒛㒞㒛㒚㒘㒝㒢㒡㒝㒟㒙㒚㒢㒞㒟㒚㒙㒟㒦㒗㒟㒣㒛㒠㒗㒠㒚㒦㒥㒞㒠㒞㒛㒞㒚㒡㒗㒟㒣㒚㒞㒚㒘㒠㒣㒟㒞㒡㒚㒙㒦㒠㒙㒥㒤㒞㒟㒞㒚㒞㒙㒡㒗㒝㒢㒠㒜㒣㒥㒥㒣㒣㒞㒗㒥㒚㒝㒢㒘㒞㒣㒞㒞㒞㒟㒥㒚㒟㒦㒛㒠㒣㒢㒦㒠㒦㒛㒞㒦㒞㒡㒞㒡㒡㒝㒣㒙㒢㒢㒡㒞㒡㒚㒝㒥㒠㒟㒣㒡㒦㒟㒡㒚㒞㒥㒞㒠㒞㒟㒟㒛㒞㒦㒗㒗㒛㒘㒝㒢㒞㒝㒞㒘㒞㒗㒟㒤㒢㒟㒢㒘㒣㒦㒤㒠㒣㒜㒜㒗㒢㒟㒦㒜㒟㒘㒜㒢㒢㒞㒚㒘㒣㒤㒠㒠㒠㒣㒢㒞㒞㒙㒞㒤㒞㒥㒥㒠㒟㒜㒛㒦㒣㒠㒥㒦㒥㒡㒞㒜㒞㒗㒞㒦㒡㒤㒗㒟㒢㒚㒗㒦㒘㒟㒣㒛㒜㒤㒥㒚㒢㒥㒞㒠㒞㒛㒞㒜㒥㒗㒟㒣㒛㒝㒣㒢㒟㒝㒥㒘㒞㒣㒞㒞㒞㒝㒦㒛㒢㒦㒢㒡㒞㒙㒥㒦㒣㒢㒢㒦㒟㒢㒟㒜㒞㒗㒞㒢㒞㒣㒝㒞㒡㒘㒛㒤㒦㒠㒚㒙㒜㒦㒜㒞㒤㒚㒥㒦㒢㒡㒣㒛㒝㒤㒟㒠㒤㒜㒚㒦㒥㒢㒥㒘㒟㒤㒚㒞㒞㒙㒞㒤㒞㒣㒟㒠㒢㒛㒢㒤㒣㒢㒦㒝㒢㒘㒠㒢㒟㒛㒡㒘㒟㒤㒡㒞㒦㒞㒛㒞㒢㒙㒞㒤㒞㒟㒞㒟㒘㒜㒡㒗㒝㒢㒜㒛㒥㒡㒤㒜㒞㒗㒞㒢㒞㒢㒛㒟㒝㒚㒜㒥㒙㒟㒣㒜㒗㒟㒟㒚㒡㒥㒞㒠㒞㒛㒞㒚㒥㒗㒣㒣㒢㒗㒟㒣㒣㒝㒞㒘㒞㒣㒞㒤㒢㒠㒗㒛㒡㒥㒡㒡㒝㒜㒠㒦㒢㒞㒜㒜㒥㒗㒥㒟㒝㒝㒥㒗㒟㒡㒣㒜㒦㒦㒠㒥㒣㒟㒘㒛㒦㒤㒣㒡㒙㒝㒠㒡㒗㒛㒞㒦㒞㒡㒞㒣㒥㒝㒣㒘㒠㒣㒦㒟㒝㒚㒝㒥㒙㒞㒗㒘㒢㒜㒦㒚㒤㒥㒞㒠㒞㒛㒞㒚㒟㒘㒛㒣㒝㒞㒣㒙㒜㒤㒢㒣㒛㒤㒘㒞㒞㒙㒞㒤㒞㒤㒡㒡㒣㒜㒠㒦㒤㒡㒟㒜㒡㒗㒣㒠㒥㒞㒣㒙㒗㒘㒛㒘㒦㒣㒞㒞㒞㒙㒞㒘㒥㒥㒣㒡㒢㒚㒛㒗㒝㒢㒣㒝㒡㒗㒣㒤㒠㒗㒦㒢㒞㒝㒞㒘㒞㒙㒠㒥㒗㒠㒢㒗㒜㒥㒠㒡㒦㒜㒝㒗㒠㒡㒘㒦㒞㒦㒥㒜㒢㒗㒞㒢㒞㒝㒞㒜㒦㒙㒣㒤㒟㒟㒢㒤㒟㒠㒗㒚㒞㒥㒞㒠㒞㒟㒠㒝㒝㒗㒢㒤㒗㒛㒤㒙㒝㒤㒠㒞㒡㒙㒣㒙㒛㒙㒤㒤㒞㒟㒞㒚㒞㒚㒠㒦㒣㒢㒛㒝㒝㒘㒢㒢㒣㒗㒟㒢㒦㒝㒞㒘㒞㒣㒞㒢㒦㒠㒣㒛㒛㒥㒟㒡㒜㒜㒝㒗㒗㒡㒢㒣㒦㒢㒢㒜㒞㒗㒞㒢㒞㒢㒡㒞㒣㒚㒢㒣㒞㒠㒠㒛㒗㒦㒛㒠㒟㒜㒠㒘㒗㒠㒞㒜㒟㒘㒠㒣㒢㒛㒡㒦㒤㒤㒠㒞㒟㒚㒛㒤㒣㒙㒟㒤㒢㒟㒞㒚㒞㒥㒞㒗㒢㒢㒗㒝㒛㒗㒣㒜㒟㒗㒢㒢㒞㒝㒞㒘㒞㒘㒞㒤㒟㒠㒠㒛㒢㒚㒛㒚㒥㒥㒞㒠㒞㒛㒞㒛㒤㒗㒣㒢㒡㒞㒢㒙㒝㒤㒠㒛㒡㒞㒛㒟㒚㒙㒞㒤㒞㒟㒞㒠㒤㒚㒗㒤㒠㒢㒤㒛㒢㒘㒚㒢㒦㒞㒡㒗㒝㒢㒡㒝㒠㒘㒝㒣㒥㒙㒢㒤㒞㒟㒞㒚㒞㒚㒚㒦㒣㒡㒤㒝㒢㒜㒛㒜㒥㒗㒞㒢㒞㒝㒞㒞㒡㒚㒝㒥㒜㒠㒜㒚㒣㒥㒡㒡㒢㒘㒚㒠㒢㒛㒞㒦㒞㒡㒞㒠㒦㒝㒣㒘㒟㒣㒢㒘㒟㒣㒦㒞㒞㒙㒞㒤㒞㒣㒠㒡㒝㒛㒢㒘㒗㒟㒥㒞㒗㒘㒠㒣㒝㒟㒠㒢㒢㒝㒞㒘㒞㒣㒞㒢㒡㒟㒟㒛㒡㒥㒦㒝㒚㒦㒛㒠㒞㒛㒞㒦㒞㒗㒟㒣㒞㒞㒗㒥㒝㒤㒥㒞㒣㒙㒠㒤㒦㒠㒝㒛㒝㒦㒙㒡㒡㒘㒝㒝㒦㒛㒠㒦㒞㒡㒞㒜㒞㒞㒝㒙㒡㒚㒦㒙㒗㒣㒞㒞㒞㒙㒞㒘㒠㒦㒝㒠㒢㒝㒗㒤㒤㒢㒝㒝㒠㒗㒡㒢㒣㒜㒥㒢㒦㒝㒞㒘㒞㒣㒞㒣㒗㒠㒜㒛㒡㒦㒢㒠㒟㒜㒜㒦㒡㒡㒣㒛㒥㒡㒡㒜㒞㒗㒞㒢㒞㒡㒣㒝㒡㒘㒞㒦㒠㒙㒤㒤㒞㒟㒞㒚㒞㒜㒡㒦㒦㒡㒟㒜㒢㒘㒝㒣㒥㒢㒛㒢㒤㒝㒞㒘㒞㒣㒞㒥㒦㒠㒞㒚㒡㒥㒟㒡㒚㒜㒚㒥㒤㒛㒞㒦㒞㒡㒞㒜㒞㒗㒞㒢㒞㒞㒢㒜㒞㒘㒥㒟㒗㒙㒞㒤㒞㒟㒞㒠㒡㒛㒦㒦㒟㒢㒠㒜㒟㒗㒡㒣㒢㒝㒣㒙㒠㒢㒥㒙㒙㒣㒞㒞㒞㒙㒞㒙㒚㒥㒣㒠㒟㒛㒢㒦㒣㒢㒠㒜㒠㒘㒝㒢㒟㒞㒠㒘㒢㒚㒦㒘㒥㒣㒞㒞㒞㒙㒞㒚㒢㒦㒗㒡㒡㒛㒡㒗㒝㒢㒠㒜㒢㒡㒟㒝㒗㒗㒞㒢㒞㒝㒞㒝㒥㒚㒝㒥㒠㒠㒙㒛㒡㒦㒞㒠㒟㒛㒡㒦㒣㒣㒠㒗㒜㒡㒞㒜㒞㒗㒞㒗㒜㒣㒣㒟㒥㒚㒢㒥㒝㒠㒜㒛㒡㒦㒝㒠㒤㒜㒢㒥㒘㒠㒡㒛㒝㒦㒜㒙㒦㒘㒘㒢㒞㒝㒞㒘㒞㒘㒙㒥㒗㒟㒡㒛㒙㒤㒞㒡㒚㒛㒟㒘㒗㒡㒣㒝㒠㒦㒥㒜㒣㒗㒞㒢㒞㒝㒞㒜㒦㒚㒝㒥㒜㒟㒣㒜㒗㒜㒦㒛㒜㒥㒞㒠㒞㒛㒞㒜㒥㒗㒟㒣㒛㒝㒣㒙㒡㒣㒣㒟㒜㒚㒡㒤㒣㒜㒝㒚㒦㒦㒢㒡㒢㒜㒞㒣㒚㒜㒙㒦㒞㒡㒞㒜㒞㒛㒡㒙㒗㒤㒢㒟㒗㒛㒘㒤㒣㒠㒜㒛㒡㒥㒦㒡㒗㒜㒞㒘㒠㒜㒘㒦㒞㒡㒞㒜㒞㒛㒥㒘㒣㒤㒢㒝㒡㒙㒣㒥㒠㒠㒤㒛㒗㒥㒡㒠㒣㒠㒛㒡㒞㒛㒞㒦㒞㒡㒞㒠㒦㒞㒣㒙㒛㒣㒟㒟㒜㒚㒝㒥㒗㒟㒢㒙㒠㒦㒝㒡㒝㒜㒢㒥㒞㒡㒟㒝㒠㒘㒢㒜㒟㒘㒘㒢㒞㒝㒞㒘㒞㒘㒘㒥㒡㒠㒝㒛㒜㒣㒢㒠㒣㒛㒡㒗㒝㒡㒢㒜㒣㒡㒟㒜㒥㒗㒞㒢㒞㒝㒞㒞㒤㒚㒠㒥㒝㒠㒛㒙㒠㒣㒥㒞㒠㒥㒟㒠㒦㒛㒞㒦㒞㒡㒞㒢㒗㒞㒗㒗㒚㒢㒣㒟㒞㒙㒝㒥㒙㒡㒗㒗㒚㒠㒟㒚㒞㒥㒞㒠㒞㒠㒠㒜㒣㒘㒞㒣㒚㒞㒗㒘㒡㒣㒟㒟㒢㒙㒣㒤㒢㒞㒡㒛㒢㒦㒝㒡㒠㒛㒟㒦㒥㒡㒣㒣㒦㒢㒙㒜㒞㒗㒞㒢㒞㒢㒚㒟㒝㒙㒡㒤㒟㒠㒚㒙㒞㒦㒚㒠㒟㒝㒗㒦㒣㒢㒠㒣㒦㒡㒢㒜㒞㒗㒞㒢㒞㒤㒥㒞㒟㒚㒗㒥㒢㒡㒠㒥㒝㒟㒞㒚㒞㒥㒞㒦㒢㒢㒡㒜㒤㒣㒞㒣㒗㒞㒡㒤㒞㒣㒦㒞㒟㒚㒠㒥㒛㒠㒚㒚㒣㒦㒡㒡㒡㒘㒚㒠㒥㒛㒞㒦㒞㒡㒞㒡㒙㒝㒣㒚㒗㒡㒢㒟㒝㒚㒥㒥㒜㒡㒠㒤㒦㒟㒞㒚㒞㒥㒞㒤㒠㒢㒝㒜㒢㒙㒗㒠㒥㒟㒗㒙㒠㒤㒝㒝㒥㒣㒣㒞㒞㒙㒞㒤㒞㒤㒛㒡㒝㒜㒜㒦㒣㒣㒗㒡㒛㒢㒙㒜㒞㒗㒞㒢㒞㒡㒟㒞㒢㒚㒛㒥㒗㒠㒜㒙㒠㒥㒣㒡㒛㒜㒝㒗㒢㒡㒣㒙㒚㒢㒚㒜㒞㒗㒞㒢㒞㒢㒗㒟㒜㒚㒤㒥㒝㒠㒙㒚㒣㒤㒡㒠㒣㒜㒠㒗㒤㒡㒣㒝㒠㒙㒠㒜㒥㒗㒞㒢㒞㒝㒞㒝㒞㒚㒚㒤㒟㒡㒗㒚㒣㒦㒠㒡㒡㒘㒚㒠㒣㒛㒞㒦㒞㒡㒞㒡㒠㒞㒗㒘㒥㒣㒦㒟㒢㒛㒠㒟㒙㒙㒞㒤㒞㒟㒞㒡㒚㒛㒣㒦㒟㒡㒢㒜㒣㒘㒠㒣㒡㒞㒢㒘㒟㒤㒢㒟㒡㒠㒦㒞㒦㒙㒞㒤㒞㒟㒞㒟㒡㒛㒡㒗㒠㒡㒣㒝㒜㒥㒥㒣㒣㒞㒗㒝㒛㒞㒙㒘㒞㒣㒞㒞㒞㒟㒡㒚㒦㒥㒣㒠㒡㒜㒙㒦㒡㒡㒟㒝㒚㒘㒚㒢㒣㒞㒠㒟㒦㒝㒥㒘㒞㒣㒞㒞㒞㒟㒦㒛㒢㒦㒢㒡㒞㒙㒘㒣㒝㒞㒝㒛㒥㒡㒣㒜㒞㒗㒞㒢㒞㒢㒡㒞㒡㒚㒝㒥㒠㒟㒣㒗㒚㒠㒗㒚㒞㒥㒞㒠㒞㒢㒥㒜㒟㒘㒚㒣㒙㒞㒡㒙㒞㒣㒣㒞㒣㒙㒢㒞㒟㒚㒦㒤㒞㒟㒞㒚㒞㒜㒞㒦㒟㒢㒡㒝㒢㒗㒣㒢㒠㒞㒗㒙㒜㒠㒜㒞㒡㒚㒝㒥㒛㒜㒝㒛㒠㒥㒟㒡㒥㒘㒝㒗㒣㒠㒙㒙㒡㒤㒥㒠㒤㒞㒘㒦㒣㒥㒠㒘㒢㒣㒞㒞㒞㒙㒞㒘㒦㒥㒣㒠㒟㒛㒢㒝㒦㒜㒘㒦㒞㒡㒞㒜㒞㒞㒗㒙㒡㒤㒚㒞㒡㒚㒚㒥㒝㒠㒡㒛㒣㒦㒠㒠㒣㒝㒠㒠㒣㒛㒞㒦㒞㒡㒞㒡㒣㒛㒢㒙㒗㒤㒛㒛㒠㒦㒚㒞㒡㒙㒞㒤㒞㒟㒞㒠㒟㒜㒞㒗㒗㒞㒚㒦㒡㒡㒞㒜㒞㒗㒞㒙㒜㒣㒣㒟㒥㒞㒛㒟㒗㒙㒞㒤㒞㒟㒞㒟㒛㒛㒟㒦㒥㒢㒜㒝㒗㒘㒢㒣㒣㒝㒢㒘㒣㒢㒥㒘㒦㒣㒞㒞㒞㒙㒞㒙㒛㒦㒝㒡㒤㒛㒣㒗㒡㒢㒞㒜㒟㒘㒛㒜㒟㒗㒢㒢㒞㒝㒞㒘㒞㒚㒞㒤㒟㒠㒠㒛㒢㒡㒚㒚㒞㒥㒞㒠㒞㒛㒠㒙㒥㒡㒞㒜㒞㒗㒞㒢㒠㒝㒞㒘㒞㒣㒞㒟㒠㒜㒤㒤㒞㒟㒞㒚㒞㒦㒛㒠㒞㒛㒞㒦㒞㒡㒞㒜㒞㒗㒞㒢㒞㒝㒞㒘㒞㒣㒞㒞㒞㒙㒞㒤㒞㒟㒞㒚㒞㒥㒟㒠㒞㒛㒞㒦㒞㒡㒞㒜㒞㒘㒠㒢㒞㒝㒞㒘㒟㒣㒞㒡㒞㒙㒞㒤㒞㒟㒞㒛㒠㒥㒞㒠㒞㒛㒟㒦㒞㒣㒚㒜㒞㒗㒞㒢㒞㒟㒤㒘㒞㒣㒞㒞㒟㒙㒞㒥㒗㒟㒞㒚㒟㒥㒞㒢㒟㒛㒞㒦㒢㒡㒡㒜㒞㒗㒞㒢㒞㒞㒗㒘㒞㒣㒟㒞㒞㒙㒞㒥㒟㒟㒞㒚㒞㒥㒞㒠㒟㒛㒞㒦㒞㒡㒞㒜㒠㒚㒥㒢㒞㒝㒟㒘㒞㒣㒟㒞㒞㒙㒞㒤㒞㒠㒠㒝㒣㒥㒞㒠㒟㒛㒞㒛㒙㒡㒞㒜㒞㒗㒞㒣㒠㒝㒞㒘㒞㒣㒟㒞㒞㒞㒜㒤㒞㒟㒞㒚㒞㒦㒠㒠㒞㒛㒞㒦㒠㒡㒞㒠㒛㒗㒞㒢㒞㒝㒞㒘㒞㒣㒞㒞㒞㒙㒟㒤㒞㒟㒠㒚㒞㒥㒟㒠㒞㒜㒠㒦㒞㒡㒞㒜㒟㒗㒞㒣㒗㒝㒞㒘㒞㒣㒞㒡㒞㒙㒞㒤㒞㒟㒟㒚㒞㒛㒢㒠㒞㒝㒥㒦㒞㒢㒠㒜㒞㒗㒞㒢㒟㒝㒞㒚㒘㒣㒞㒞㒞㒙㒞㒦㒞㒟㒞㒚㒞㒥㒟㒠㒞㒛㒟㒦㒞㒢㒘㒜㒞㒘㒠㒢㒞㒝㒞㒘㒡㒣㒞㒣㒣㒙㒞㒤㒞㒟㒞㒚㒞㒥㒞㒠㒞㒛㒟㒦㒞㒡㒡㒜㒞㒗㒠㒢㒞㒟㒞㒚㒛㒣㒞㒞㒟㒙㒞㒤㒟㒟㒞㒟㒛㒥㒞㒢㒞㒝㒟㒦㒞㒡㒠㒜㒞㒗㒟㒢㒞㒟㒣㒘㒞㒣㒞㒠㒦㒙㒞㒤㒠㒟㒞㒚㒠㒥㒞㒠㒠㒛㒞㒘㒞㒣㒛㒜㒞㒗㒡㒢㒞㒝㒠㒘㒞㒘㒞㒞㒞㒛㒞㒦㒟㒟㒞㒚㒡㒥㒞㒠㒡㒛㒞㒙㒠㒡㒞㒜㒠㒚㒥㒢㒞㒝㒣㒘㒞㒣㒞㒞㒞㒙㒞㒤㒞㒟㒞㒛㒞㒥㒞㒠㒡㒛㒞㒦㒣㒡㒞㒜㒟㒗㒞㒢㒞㒞㒟㒘㒞㒣㒞㒞㒞㒙㒟㒤㒞㒟㒞㒚㒞㒥㒞㒠㒡㒛㒞㒦㒞㒡㒞㒞㒚㒗㒞㒢㒞㒝㒞㒝㒥㒣㒢㒞㒞㒙㒞㒤㒞㒤㒜㒠㒟㒜㒛㒦㒣㒙㒙㒦㒞㒡㒟㒝㒙㒗㒞㒢㒞㒝㒞㒝㒚㒚㒝㒤㒡㒟㒟㒛㒚㒤㒞㒡㒚㒛㒟㒘㒗㒡㒣㒝㒠㒤㒚㒜㒣㒗㒞㒢㒞㒝㒞㒝㒛㒘㒡㒣㒙㒟㒣㒜㒗㒗㒠㒚㒣㒥㒞㒠㒞㒛㒞㒛㒛㒘㒝㒣㒤㒝㒣㒥㒡㒚㒦㒘㒥㒣㒞㒞㒞㒙㒞㒙㒞㒦㒚㒠㒟㒝㒗㒦㒣㒢㒠㒝㒡㒦㒥㒜㒣㒗㒞㒢㒞㒝㒞㒝㒛㒚㒝㒥㒤㒟㒣㒗㒥㒟㒟㒚㒦㒥㒞㒠㒞㒛㒞㒛㒛㒘㒝㒣㒤㒝㒣㒙㒡㒤㒞㒞㒟㒚㒛㒙㒛㒙㒦㒤㒞㒟㒞㒚㒞㒙㒠㒦㒟㒡㒡㒝㒙㒘㒞㒢㒟㒝㒡㒙㒙㒝㒟㒘㒣㒣㒞㒞㒞㒙㒞㒙㒛㒦㒝㒡㒤㒛㒣㒣㒣㒣㒠㒗㒗㒡㒞㒜㒞㒗㒞㒗㒥㒤㒝㒟㒠㒚㒙㒥㒡㒠㒞㒚㒟㒥㒡㒠㒣㒢㒦㒡㒙㒛㒞㒦㒞㒡㒞㒠㒥㒝㒣㒙㒢㒡㒡㒞㒦㒚㒗㒥㒚㒟㒢㒛㒠㒥㒣㒡㒜㒛㒘㒠㒟㒞㒚㒦㒣㒡㒞㒜㒞㒗㒞㒗㒛㒤㒝㒟㒤㒙㒣㒡㒠㒙㒟㒤㒣㒟㒞㒚㒞㒥㒞㒥㒛㒢㒝㒝㒤㒗㒣㒟㒦㒢㒛㒢㒢㒝㒞㒘㒞㒣㒞㒤㒥㒟㒟㒛㒛㒥㒣㒝㒚㒥㒦㒠㒞㒛㒞㒦㒞㒥㒟㒢㒡㒞㒢㒙㒗㒤㒤㒞㒟㒚㒢㒤㒣㒜㒚㒤㒣㒟㒞㒚㒞㒥㒞㒗㒞㒡㒟㒝㒗㒘㒠㒣㒡㒢㒛㒢㒢㒝㒞㒘㒞㒣㒞㒥㒥㒟㒟㒛㒗㒦㒢㒚㒟㒥㒤㒠㒞㒛㒞㒦㒞㒦㒞㒢㒟㒞㒠㒘㒣㒤㒜㒟㒢㒣㒟㒞㒣㒙㒞㒤㒞㒟㒞㒟㒛㒜㒝㒗㒤㒡㒣㒙㒟㒙㒠㒜㒣㒗㒞㒢㒞㒝㒞㒝㒛㒚㒝㒥㒤㒟㒣㒘㒗㒜㒦㒚㒣㒥㒞㒠㒞㒛㒞㒛㒛㒘㒝㒣㒤㒝㒣㒥㒢㒚㒦㒘㒢㒣㒞㒞㒞㒙㒞㒛㒜㒥㒟㒡㒛㒛㒣㒣㒚㒛㒠㒦㒞㒡㒞㒜㒞㒝㒝㒦㒥㒘㒛㒘㒢㒣㒞㒞㒞㒙㒞㒙㒚㒦㒗㒡㒤㒛㒣㒥㒥㒛㒣㒦㒞㒡㒞㒜㒞㒜㒛㒙㒝㒤㒤㒞㒣㒦㒤㒞㒟㒚㒘㒤㒞㒟㒞㒚㒞㒙㒢㒦㒣㒡㒟㒜㒡㒘㒢㒣㒗㒞㒤㒘㒟㒤㒢㒞㒣㒙㒟㒞㒞㒙㒞㒤㒞㒠㒠㒝㒦㒥㒞㒠㒟㒛㒞㒘㒗㒡㒞㒜㒞㒗㒞㒤㒞㒟㒛㒘㒞㒣㒟㒞㒞㒙㒟㒤㒞㒟㒦㒚㒞㒥㒤㒥㒙㒛㒞㒦㒟㒡㒞㒝㒘㒗㒞㒢㒟㒝㒞㒘㒞㒣㒞㒞㒢㒙㒡㒤㒞㒟㒞㒚㒞㒦㒘㒠㒞㒛㒟㒦㒞㒢㒠㒟㒦㒗㒞㒢㒟㒝㒞㒘㒢㒣㒞㒞㒞㒙㒞㒤㒤㒠㒚㒚㒞㒥㒞㒠㒞㒜㒘㒦㒞㒡㒟㒜㒞㒗㒟㒢㒞㒝㒢㒘㒡㒣㒞㒞㒞㒙㒞㒥㒘㒟㒞㒚㒟㒥㒞㒡㒠㒞㒦㒦㒞㒡㒟㒜㒞㒙㒗㒢㒞㒝㒞㒘㒞㒦㒞㒡㒠㒙㒞㒤㒟㒟㒞㒚㒦㒥㒞㒠㒠㒛㒞㒦㒢㒡㒡㒜㒞㒗㒞㒢㒞㒣㒞㒘㒞㒣㒟㒞㒞㒚㒠㒗㒦㒟㒞㒚㒟㒥㒞㒢㒗㒛㒞㒦㒞㒡㒞㒞㒞㒙㒛㒢㒞㒝㒟㒘㒞㒣㒟㒞㒞㒙㒦㒤㒞㒡㒤㒝㒜㒥㒞㒠㒟㒛㒞㒗㒝㒡㒞㒜㒟㒗㒞㒢㒠㒝㒞㒘㒢㒣㒡㒞㒞㒙㒞㒤㒞㒠㒝㒚㒞㒥㒟㒠㒞㒛㒢㒦㒡㒡㒞㒜㒞㒗㒞㒘㒞㒝㒞㒘㒟㒣㒞㒟㒠㒜㒦㒤㒞㒟㒟㒚㒞㒥㒢㒠㒞㒛㒞㒦㒞㒡㒤㒝㒚㒗㒞㒢㒞㒝㒞㒞㒞㒣㒞㒞㒟㒙㒞㒤㒟㒟㒞㒚㒢㒥㒡㒠㒞㒛㒞㒦㒞㒗㒞㒜㒞㒗㒟㒢㒞㒞㒠㒛㒦㒣㒞㒞㒟㒙㒞㒦㒗㒟㒞㒚㒞㒥㒞㒣㒞㒞㒠㒦㒞㒡㒟㒜㒞㒗㒦㒢㒞㒞㒛㒘㒞㒤㒠㒡㒦㒙㒞㒤㒟㒟㒞㒜㒗㒥㒞㒠㒞㒛㒞㒘㒞㒣㒛㒜㒞㒗㒟㒢㒞㒝㒟㒘㒞㒣㒦㒞㒞㒙㒤㒙㒙㒟㒞㒚㒟㒥㒞㒦㒞㒛㒞㒦㒟㒡㒞㒜㒞㒗㒞㒢㒢㒝㒡㒘㒞㒣㒞㒞㒞㒟㒞㒤㒞㒟㒟㒚㒞㒦㒠㒣㒦㒛㒞㒦㒟㒡㒞㒝㒠㒗㒞㒢㒞㒝㒞㒙㒠㒥㒤㒞㒞㒙㒠㒤㒞㒠㒞㒚㒞㒥㒞㒠㒞㒝㒞㒦㒞㒡㒞㒜㒠㒗㒞㒢㒠㒝㒞㒘㒤㒣㒞㒠㒞㒙㒞㒤㒞㒟㒠㒚㒞㒥㒠㒠㒞㒛㒡㒦㒞㒣㒞㒜㒞㒗㒞㒢㒠㒝㒞㒘㒠㒣㒞㒟㒗㒙㒞㒦㒞㒟㒞㒚㒞㒥㒠㒠㒞㒛㒠㒦㒞㒢㒚㒜㒞㒗㒞㒢㒞㒝㒞㒘㒠㒣㒞㒞㒡㒙㒞㒤㒞㒟㒞㒚㒞㒥㒞㒠㒞㒛㒟㒦㒞㒡㒞㒜㒞㒗㒡㒢㒞㒝㒢㒘㒞㒣㒞㒞㒞㒙㒞㒚㒛㒟㒞㒚㒟㒥㒞㒢㒞㒝㒛㒦㒞㒡㒤㒜㒞㒗㒣㒢㒞㒝㒟㒘㒞㒤㒠㒡㒦㒙㒞㒤㒥㒟㒞㒛㒣㒥㒞㒠㒞㒛㒞㒦㒤㒣㒝㒜㒞㒗㒤㒢㒞㒢㒗㒘㒞㒣㒟㒞㒞㒙㒥㒤㒞㒟㒢㒚㒡㒥㒞㒠㒞㒛㒞㒛㒗㒡㒞㒜㒟㒗㒞㒤㒞㒟㒛㒘㒞㒣㒤㒞㒞㒙㒣㒤㒞㒟㒟㒚㒞㒦㒠㒣㒦㒛㒞㒦㒥㒡㒞㒝㒜㒗㒞㒢㒞㒝㒞㒘㒤㒥㒝㒞㒞㒙㒤㒤㒞㒤㒗㒚㒞㒥㒟㒠㒞㒛㒥㒦㒞㒡㒢㒜㒡㒗㒞㒢㒞㒝㒞㒝㒗㒣㒞㒞㒟㒙㒞㒦㒞㒡㒛㒚㒞㒥㒤㒠㒞㒛㒣㒦㒞㒡㒟㒜㒞㒘㒠㒥㒦㒝㒞㒘㒥㒣㒞㒞㒣㒙㒞㒤㒞㒟㒞㒚㒤㒦㒚㒠㒞㒛㒤㒦㒞㒤㒜㒜㒞㒗㒟㒢㒞㒝㒥㒘㒞㒣㒢㒞㒡㒙㒞㒤㒞㒟㒞㒝㒜㒥㒞㒠㒟㒛㒞㒦㒢㒡㒡㒜㒞㒗㒞㒢㒞㒢㒗㒘㒞㒣㒟㒞㒞㒛㒞㒦㒛㒟㒞㒚㒤㒥㒞㒠㒣㒛㒞㒦㒟㒡㒞㒝㒠㒚㒦㒢㒞㒝㒥㒘㒞㒤㒥㒞㒞㒙㒞㒤㒞㒟㒤㒜㒝㒥㒞㒠㒤㒛㒞㒛㒗㒡㒞㒜㒟㒗㒞㒢㒥㒝㒞㒘㒢㒣㒡㒞㒞㒙㒞㒤㒞㒤㒗㒚㒞㒥㒟㒠㒞㒝㒞㒘㒛㒡㒞㒜㒤㒗㒞㒢㒣㒝㒞㒘㒟㒣㒞㒟㒠㒜㒦㒤㒞㒟㒥㒚㒞㒦㒘㒠㒞㒛㒞㒦㒞㒡㒤㒝㒚㒗㒞㒢㒤㒝㒞㒛㒥㒣㒞㒞㒟㒙㒞㒤㒥㒟㒞㒚㒢㒥㒡㒠㒞㒛㒞㒦㒞㒤㒥㒜㒞㒗㒟㒢㒞㒝㒢㒘㒡㒣㒞㒞㒞㒙㒞㒙㒗㒟㒞㒚㒟㒥㒞㒢㒞㒝㒛㒦㒞㒡㒤㒜㒞㒗㒣㒢㒞㒝㒟㒘㒞㒤㒠㒡㒦㒙㒞㒤㒥㒟㒞㒜㒙㒥㒞㒠㒞㒛㒞㒦㒤㒣㒝㒜㒞㒗㒤㒢㒞㒢㒗㒘㒞㒣㒟㒞㒞㒙㒥㒤㒞㒟㒢㒚㒡㒥㒞㒠㒞㒛㒞㒛㒗㒡㒞㒜㒟㒗㒞㒤㒞㒟㒛㒘㒞㒣㒤㒞㒞㒙㒣㒤㒞㒟㒟㒚㒞㒦㒠㒣㒦㒛㒞㒦㒥㒡㒞㒜㒥㒗㒞㒢㒞㒝㒞㒘㒤㒤㒚㒞㒞㒙㒤㒤㒞㒣㒞㒚㒞㒥㒟㒠㒞㒛㒥㒦㒞㒡㒢㒜㒡㒗㒞㒢㒞㒝㒞㒜㒞㒣㒞㒞㒟㒙㒞㒤㒢㒟㒡㒚㒞㒥㒞㒠㒞㒠㒗㒦㒞㒡㒟㒜㒞㒙㒞㒤㒛㒝㒞㒘㒤㒣㒞㒞㒣㒙㒞㒤㒟㒟㒞㒛㒠㒘㒦㒠㒞㒛㒥㒦㒞㒢㒝㒜㒞㒗㒞㒢㒞㒝㒤㒚㒝㒣㒞㒞㒤㒙㒞㒙㒗㒟㒞㒚㒟㒥㒞㒠㒥㒛㒞㒦㒢㒡㒡㒜㒞㒗㒞㒢㒞㒢㒗㒘㒞㒣㒟㒞㒞㒛㒞㒦㒛㒟㒞㒚㒤㒥㒞㒠㒣㒛㒞㒦㒟㒡㒞㒝㒠㒚㒦㒢㒞㒝㒥㒘㒞㒤㒤㒞㒞㒙㒞㒤㒞㒟㒤㒜㒝㒥㒞㒠㒤㒛㒞㒛㒗㒡㒞㒜㒟㒗㒞㒢㒥㒝㒞㒘㒢㒣㒡㒞㒞㒙㒞㒤㒞㒤㒗㒚㒞㒥㒟㒠㒞㒛㒢㒦㒡㒡㒞㒜㒞㒗㒞㒘㒛㒝㒞㒘㒟㒣㒞㒟㒠㒜㒦㒤㒞㒟㒤㒚㒞㒦㒞㒠㒞㒛㒞㒦㒞㒣㒞㒟㒘㒗㒞㒢㒤㒝㒞㒘㒤㒣㒞㒟㒙㒙㒞㒦㒞㒟㒞㒚㒞㒥㒤㒠㒞㒛㒤㒦㒞㒣㒘㒜㒞㒘㒠㒢㒞㒝㒞㒘㒥㒣㒞㒟㒞㒙㒞㒤㒞㒟㒞㒜㒞㒥㒞㒠㒞㒛㒥㒦㒞㒡㒥㒜㒞㒗㒤㒢㒞㒟㒞㒘㒞㒣㒞㒞㒥㒙㒞㒤㒥㒟㒞㒚㒡㒥㒞㒢㒞㒛㒞㒦㒞㒡㒥㒜㒞㒗㒥㒢㒞㒞㒦㒘㒞㒣㒞㒞㒞㒙㒞㒤㒤㒟㒞㒚㒤㒥㒞㒠㒥㒛㒞㒗㒞㒡㒞㒜㒞㒗㒣㒢㒞㒞㒢㒘㒞㒣㒤㒞㒞㒛㒞㒤㒞㒟㒞㒚㒤㒥㒞㒠㒣㒛㒞㒗㒟㒡㒞㒜㒞㒗㒞㒢㒞㒝㒤㒘㒞㒣㒠㒞㒞㒙㒟㒤㒞㒡㒞㒚㒞㒥㒞㒠㒤㒛㒞㒦㒣㒡㒞㒞㒚㒗㒞㒢㒞㒝㒞㒘㒞㒣㒤㒞㒞㒙㒠㒤㒞㒟㒟㒚㒞㒦㒠㒠㒞㒛㒞㒦㒤㒡㒞㒝㒡㒗㒞㒢㒞㒝㒞㒘㒞㒣㒞㒞㒞㒙㒤㒤㒞㒟㒟㒚㒞㒥㒟㒠㒞㒜㒠㒦㒞㒡㒞㒜㒤㒗㒞㒣㒞㒝㒞㒘㒞㒣㒞㒠㒞㒙㒞㒤㒞㒟㒤㒚㒞㒥㒤㒠㒞㒛㒤㒦㒞㒣㒞㒜㒞㒗㒞㒢㒤㒝㒞㒘㒤㒣㒞㒞㒡㒙㒞㒦㒞㒟㒞㒚㒞㒥㒤㒠㒞㒛㒤㒦㒞㒢㒗㒜㒞㒘㒞㒢㒞㒝㒞㒘㒣㒣㒞㒟㒢㒙㒞㒤㒤㒟㒞㒚㒤㒚㒗㒠㒞㒛㒟㒦㒞㒣㒟㒜㒞㒗㒟㒢㒞㒝㒠㒘㒞㒣㒢㒞㒡㒙㒞㒤㒞㒟㒞㒜㒟㒥㒞㒠㒟㒛㒞㒦㒢㒡㒡㒜㒞㒗㒞㒢㒞㒞㒢㒘㒞㒣㒟㒞㒞㒙㒞㒥㒟㒟㒞㒚㒞㒥㒞㒠㒟㒛㒞㒦㒞㒡㒞㒜㒟㒗㒞㒢㒞㒝㒞㒘㒞㒣㒦㒞㒞㒙㒞㒤㒞㒤㒤㒚㒞㒥㒞㒠㒞㒛㒞㒦㒞㒡㒞㒛㒞㒛㒝㒟㒥㒝㒞㒘㒞㒣㒞㒞㒞㒙㒞㒤㒞㒦㒞㒞㒞㒝㒠㒠㒢㒛㒞㒦㒞㒡㒞㒢㒠㒟㒗㒙㒢㒣㒣㒘㒟㒣㒞㒞㒞㒙㒞㒤㒞㒟㒟㒚㒤㒥㒞㒠㒞㒛㒞㒝㒡㒘㒢㒣㒠㒞㒗㒙㒜㒣㒥㒘㒟㒣㒡㒞㒞㒙㒞㒤㒞㒦㒡㒡㒣㒛㒠㒣㒚㒜㒚㒦㒞㒡㒞㒜㒞㒝㒤㒗㒗㒡㒠㒟㒤㒘㒢㒥㒚㒟㒦㒛㒡㒤㒝㒟㒡㒚㒠㒥㒝㒠㒥㒦㒢㒡㒞㒜㒞㒗㒞㒘㒡㒣㒦㒞㒟㒚㒠㒠㒠㒙㒞㒤㒞㒟㒞㒛㒠㒘㒦㒠㒞㒛㒡㒦㒞㒡㒥㒜㒞㒗㒞㒢㒞㒝㒞㒙㒠㒣㒞㒞㒡㒙㒞㒤㒡㒟㒞㒚㒟㒥㒞㒠㒤㒛㒥㒦㒞㒡㒡㒜㒞㒗㒣㒢㒞㒝㒟㒘㒞㒣㒟㒞㒞㒙㒢㒤㒡㒟㒞㒚㒞㒥㒞㒠㒣㒛㒞㒦㒟㒡㒞㒜㒢㒗㒡㒢㒞㒝㒞㒘㒞㒣㒦㒞㒞㒙㒟㒤㒞㒠㒠㒝㒦㒥㒞㒠㒡㒛㒞㒦㒥㒡㒞㒜㒞㒗㒞㒢㒞㒞㒠㒘㒞㒣㒡㒞㒞㒙㒡㒤㒞㒟㒟㒚㒞㒥㒞㒥㒣㒛㒞㒦㒡㒡㒞㒜㒠㒗㒞㒢㒞㒝㒞㒙㒠㒗㒞㒞㒞㒙㒡㒤㒞㒟㒟㒚㒞㒥㒞㒠㒞㒜㒠㒚㒜㒡㒞㒜㒢㒗㒞㒢㒢㒝㒞㒘㒞㒣㒞㒟㒠㒙㒞㒤㒞㒟㒣㒚㒞㒥㒟㒠㒞㒛㒞㒦㒞㒡㒞㒜㒞㒗㒞㒢㒤㒝㒞㒘㒞㒣㒞㒞㒞㒙㒞㒥㒠㒟㒞㒚㒞㒥㒥㒠㒞㒛㒟㒦㒞㒡㒞㒜㒞㒗㒢㒢㒞㒝㒞㒘㒣㒣㒞㒠㒜㒙㒞㒤㒟㒟㒞㒚㒞㒦㒢㒠㒞㒜㒗㒦㒞㒡㒢㒜㒞㒗㒞㒢㒞㒞㒠㒚㒚㒣㒞㒟㒘㒙㒞㒤㒣㒟㒞㒚㒞㒥㒞㒢㒞㒛㒞㒦㒞㒢㒘㒜㒞㒘㒘㒢㒞㒝㒦㒘㒞㒥㒞㒞㒞㒙㒞㒥㒙㒟㒞㒚㒞㒥㒞㒠㒤㒛㒞㒦㒞㒡㒞㒜㒞㒘㒛㒢㒞㒝㒦㒘㒞㒣㒞㒞㒞㒙㒞㒤㒞㒟㒞㒛㒜㒥㒞㒠㒦㒛㒞㒦㒞㒡㒞㒜㒞㒗㒞㒢㒞㒞㒙㒘㒞㒤㒜㒞㒞㒙㒠㒤㒞㒡㒞㒚㒞㒥㒞㒡㒙㒛㒞㒗㒙㒡㒞㒜㒡㒗㒞㒢㒞㒝㒞㒘㒞㒤㒙㒞㒞㒙㒠㒤㒞㒟㒠㒚㒞㒥㒞㒠㒞㒛㒞㒗㒙㒡㒞㒝㒙㒗㒞㒢㒡㒝㒞㒚㒞㒣㒞㒞㒞㒚㒙㒤㒞㒠㒙㒚㒞㒥㒠㒠㒞㒛㒞㒦㒞㒡㒞㒝㒘㒗㒞㒢㒠㒝㒞㒘㒠㒣㒞㒞㒞㒙㒞㒤㒞㒟㒢㒚㒞㒦㒗㒠㒞㒜㒘㒦㒞㒡㒞㒜㒞㒗㒞㒣㒗㒝㒞㒘㒡㒣㒞㒞㒠㒙㒞㒦㒞㒟㒞㒚㒞㒥㒡㒠㒞㒜㒗㒦㒞㒡㒠㒜㒞㒗㒢㒤㒜㒝㒞㒘㒣㒣㒞㒟㒜㒙㒞㒤㒟㒟㒞㒛㒠㒘㒦㒠㒞㒛㒣㒦㒞㒡㒥㒜㒞㒗㒞㒢㒞㒝㒞㒜㒡㒣㒞㒞㒣㒙㒞㒤㒟㒟㒞㒚㒢㒥㒞㒠㒞㒠㒣㒦㒞㒡㒢㒜㒞㒗㒠㒢㒞㒝㒞㒘㒞㒣㒞㒟㒟㒙㒞㒤㒞㒟㒞㒚㒟㒥㒞㒠㒞㒛㒞㒦㒡㒡㒞㒜㒞㒗㒞㒢㒞㒝㒠㒘㒞㒣㒞㒞㒞㒤㒛㒤㒣㒟㒞㒚㒞㒥㒞㒗㒞㒡㒡㒜㒟㒘㒚㒣㒚㒗㒞㒢㒞㒝㒞㒘㒞㒣㒞㒞㒞㒙㒞㒤㒞㒟㒞㒜㒜㒥㒞㒠㒞㒛㒞㒗㒠㒥㒞㒜㒞㒗㒠㒢㒞㒝㒠㒘㒞㒣㒞㒞㒞㒚㒠㒘㒞㒟㒞㒚㒡㒥㒞㒠㒠㒛㒞㒦㒞㒡㒞㒝㒠㒚㒦㒢㒞㒝㒢㒘㒞㒣㒟㒞㒞㒙㒞㒤㒞㒟㒤㒞㒠㒥㒞㒠㒣㒛㒞㒦㒞㒡㒞㒜㒟㒗㒞㒢㒢㒝㒞㒘㒞㒦㒚㒞㒞㒙㒞㒤㒞㒟㒠㒚㒞㒥㒞㒠㒞㒛㒞㒙㒚㒡㒞㒜㒞㒗㒞㒢㒞㒝㒞㒘㒞㒣㒞㒞㒞㒜㒚㒤㒞㒟㒞㒚㒞㒥㒡㒠㒞㒛㒞㒦㒞㒡㒞㒟㒚㒗㒞㒢㒞㒝㒞㒘㒟㒣㒞㒞㒞㒙㒞㒤㒞㒤㒝㒚㒞㒥㒢㒠㒞㒛㒠㒦㒞㒡㒟㒜㒞㒗㒤㒤㒝㒝㒞㒘㒞㒣㒞㒟㒚㒙㒞㒤㒟㒟㒞㒚㒟㒥㒞㒠㒢㒛㒡㒦㒞㒡㒞㒜㒞㒘㒚㒢㒞㒝㒟㒘㒞㒣㒢㒞㒡㒙㒞㒤㒞㒟㒞㒜㒘㒥㒞㒠㒟㒛㒞㒦㒤㒣㒝㒜㒞㒗㒞㒢㒞㒞㒝㒘㒞㒣㒟㒞㒞㒙㒟㒤㒞㒟㒢㒚㒡㒥㒞㒠㒞㒛㒞㒗㒝㒡㒞㒜㒟㒗㒞㒢㒢㒝㒡㒘㒞㒣㒞㒞㒞㒛㒘㒤㒞㒟㒟㒚㒞㒥㒤㒢㒝㒛㒞㒦㒟㒡㒞㒝㒠㒗㒞㒢㒟㒝㒞㒘㒞㒣㒞㒞㒢㒙㒡㒤㒞㒟㒞㒚㒞㒦㒠㒠㒞㒛㒟㒦㒞㒡㒢㒜㒡㒗㒞㒢㒞㒝㒞㒚㒘㒣㒞㒞㒟㒙㒞㒤㒞㒤㒟㒚㒞㒥㒢㒠㒞㒛㒠㒦㒞㒡㒡㒜㒞㒗㒞㒗㒟㒝㒞㒘㒣㒣㒞㒞㒡㒙㒞㒤㒠㒟㒞㒚㒤㒦㒚㒠㒞㒛㒢㒦㒞㒣㒘㒜㒞㒗㒟㒢㒞㒝㒣㒘㒞㒣㒢㒞㒡㒙㒞㒤㒞㒟㒞㒜㒘㒥㒞㒠㒟㒛㒞㒦㒞㒦㒟㒜㒞㒗㒢㒢㒞㒝㒠㒘㒞㒣㒡㒞㒞㒙㒞㒙㒟㒟㒞㒚㒣㒥㒞㒠㒡㒛㒞㒦㒠㒡㒞㒜㒤㒙㒝㒢㒞㒝㒢㒘㒞㒥㒙㒞㒞㒙㒟㒤㒞㒟㒣㒚㒞㒥㒢㒠㒡㒛㒞㒦㒞㒡㒞㒞㒙㒗㒞㒢㒟㒝㒞㒘㒞㒘㒢㒞㒞㒙㒢㒤㒞㒟㒞㒚㒞㒥㒞㒠㒞㒛㒞㒙㒗㒡㒞㒜㒢㒗㒞㒢㒟㒝㒞㒘㒞㒣㒞㒞㒞㒞㒣㒤㒞㒟㒢㒚㒞㒥㒠㒠㒞㒛㒞㒦㒞㒡㒞㒝㒟㒗㒞㒢㒞㒝㒞㒘㒟㒣㒞㒞㒞㒙㒞㒤㒠㒟㒟㒚㒞㒥㒞㒠㒞㒛㒞㒦㒞㒡㒞㒜㒞㒗㒥㒢㒞㒝㒞㒘㒞㒣㒞㒞㒤㒙㒞㒤㒞㒟㒞㒚㒟㒥㒞㒠㒞㒛㒞㒦㒞㒡㒞㒜㒞㒗㒞㒢㒞㒝㒞㒘㒞㒣㒞㒞㒞㒙㒞㒤㒞㒟㒞㒚㒞㒥㒞㒠㒞㒛㒞㒦㒞㒡㒞㒜㒞㒗㒞㒢㒞㒝㒞㒘㒞㒣㒡㒞㒞㒙㒞㒤㒞㒟㒞㒚㒞㒥㒞㒠㒞㒛㒞㒦㒞㒡㒞㒜㒞㒗㒞㒢㒞㒝㒞㒘㒞㒣㒞㒞㒞㒙㒠㒤㒞㒟㒞㒚㒞㒥㒞㒠㒞㒛㒞㒦㒞㒡㒞㒜㒟㒗㒞㒢㒞㒝㒞㒘㒞㒣㒞㒞㒞㒙㒞㒤㒞");local _l_ll=(0xdf-(146+-#{(function()return{','}end)(),76;{}}))local _ll=105 local __=__l;local _={}_={[((6080/0x98)+-#"I have 0x in my nickname and I am cool.")]=function()local _lll,__l,_l,_=___lll(__l_ll,__,__+__l__);__=__+_ll__;_ll=(_ll+(_l_ll*_ll__))%_l_;return(((_+_ll-(_l_ll)+___*(_ll__*__ll))%___)*((__ll*_ll_ll)^__ll))+(((_l+_ll-(_l_ll*__ll)+___*(__ll^__l__))%_l_)*(___*_l_))+(((__l+_ll-(_l_ll*__l__)+_ll_ll)%_l_)*___)+((_lll+_ll-(_l_ll*_ll__)+_ll_ll)%_l_);end,[(-#"<@!761654159095103499> send toe nail pics"+(0x95-106))]=function(_,_,_)local _=___lll(__l_ll,__,__);__=__+_lll;_ll=(_ll+(_l_ll))%_l_;return((_+_ll-(_l_ll)+_ll_ll)%___);end,[(0x24+-33)]=function()local _l,_=___lll(__l_ll,__,__+__ll);_ll=(_ll+(_l_ll*__ll))%_l_;__=__+__ll;return(((_+_ll-(_l_ll)+___*(__ll*_ll__))%___)*_l_)+((_l+_ll-(_l_ll*__ll)+_l_*(__ll^__l__))%___);end,[(0x51-77)]=function(__,_,_l)if _l then local _=(__/__ll^(_-__l))%__ll^((_l-_lll)-(_-__l)+_lll);return _-_%__l;else local _=__ll^(_-_lll);return(__%(_+_)>=_)and __l or _____;end;end,[((0x8a0/48)+-#[[MoonSec V3 cracked download not clickbait]])]=function()local _l=_[(0x4d/77)]();local __=_[(-0x57+88)]();local _l_l=__l;local _ll=(_[(0x21-29)](__,_lll,_l_lll+_ll__)*(__ll^(_l_lll*__ll)))+_l;local _l=_[(-0x55+89)](__,21,31);local _=((-__l)^_[(-106+0x6e)](__,32));if(_l==_____)then if(_ll==_lllll)then return _*_____;else _l=_lll;_l_l=_lllll;end;elseif(_l==(___*(__ll^__l__))-_lll)then return(_ll==_____)and(_*(_lll/_lllll))or(_*(_____/_lllll));end;return _ll__l(_,_l-((_l_*(_ll__))-__l))*(_l_l+(_ll/(__ll^___l_l)));end,[(0x108/44)]=function(_l,__ll,__ll)local __ll;if(not _l)then _l=_[(0x2b/43)]();if(_l==_____)then return'';end;end;__ll=_l_l_l(__l_ll,__,__+_l-__l);__=__+_l;local _=''for _l=_lll,#__ll do _=__ll_l(_,_l__ll((___lll(_l_l_l(__ll,_l,_l))+_ll)%_l_))_ll=(_ll+_l_ll)%___ end return _;end}local function __l_ll(...)return{...},____ll('#',...)end local function _ll_ll()local _llll={};local __l_={};local _l={};local __lll={_llll,__l_,nil,_l};local __={}local _l_ll=(0x73-92)local _ll={[(872/((-112+0x17a)+-#[[Fun and games until a = (function() a() end) a()]]))]=(function(_l)return not(#_l==_[((128-0x62)+-#[[FEDERAL IS A FUCKING SCAMMER]])]())end),[(-0x77+119)]=(function(_l)return _[(0x28+-35)]()end),[(-#"staymad"+(0x38-48))]=(function(_l)return _[(126/0x15)]()end),[(-#"i love perth"+(0xa8/12))]=(function(_l)local __=_[(34-0x1c)]()local _=''local _l=1 for _ll=1,#__ do _l=(_l+_l_ll)%_l_ _=__ll_l(_,_l__ll((___lll(__:sub(_ll,_ll))+_l)%___))end return _ end)};local _l=_[(42-0x29)]()for _l=1,_l do local _=_[(-#[[This file has been enchanted with uncrackable V, fuck the fuck off]]+(-84+0x98))]();local __l;local _=_ll[_%(387/0x9)];__[_l]=_ and _({});end;for __l_=1,_[(97/0x61)]()do local _l=_[(113-0x6f)]();if(_[(-90+0x5e)](_l,__l,_lll)==_lllll)then local _l_=_[(34-0x1e)](_l,__ll,__l__);local _ll=_[(1012/0xfd)](_l,_ll__,__ll+_ll__);local _l={_[(0x195/((33124/0xa9)+-#'psu got dumped so hard their entire source code came out rofl'))](),_[(-#"Pain is an illusion created by your brain"+(0xfd0/92))](),nil,nil};local ___={[(0x5a+-90)]=function()_l[__l_l]=_[(-#'fortnite balls'+(0x693/99))]();_l[_lll_]=_[(-#[[<@!519139355118534656> stop with the cap ms v3 got my script 30.0 ms]]+(0xb5f/41))]();end,[((0xb1-137)+-#'i know what sex is, but i wont tell you')]=function()_l[_l_l]=_[(-#'Shouldve invite FBI Bot'+(117-0x5d))]();end,[((0x70c/41)+-#[[pssssst the wrapper function is over there]])]=function()_l[_l_l]=_[(0xc8/200)]()-(__ll^_l_lll)end,[(27-0x18)]=function()_l[____]=_[(98/0x62)]()-(__ll^_l_lll)_l[_l___]=_[(0x27-36)]();end};___[_l_]();if(_[((0x3f+-16)+-#[[Imagine being named omer faruk birer aka RY]])](_ll,_lll,__l)==_lll)then _l[_ll_]=__[_l[___l]]end if(_[((0x63+-82)+-#"bit.bdiv(0,0)")](_ll,__ll,__ll)==__l)then _l[_ll_l]=__[_l[_l__]]end if(_[(0x48+(-17000/0xfa))](_ll,__l__,__l__)==_lll)then _l[__ll_]=__[_l[_lll_]]end _llll[__l_]=_l;end end;__lll[3]=_[((-0x2b+57)+-#[[mom shot dad]])]();for _=_lll,_[((10478/0xa9)+-#[[psu got dumped so hard their entire source code came out rofl]])]()do __l_[_-_lll]=_ll_ll();end;return __lll;end;local function _____(_,_ll__,_l_ll)local __=_[__ll];local _l_=_[__l__];local _=_[__l];return(function(...)local _l__ll={};local ___=_;local ___lll=__l_ll local _ll=__l;local _lllll=__;local __={};local _=__l _*=-1 local __l__=_;local _l_lll={};local __l_ll=____ll('#',...)-_lll;local _ll_ll={...};local _l_=_l_;for _=0,__l_ll do if(_>=_l_)then _l__ll[_-_l_]=_ll_ll[_+_lll];else __[_]=_ll_ll[_+__l];end;end;local _=__l_ll-_l_+__l local _;local _l_;while true do _=___[_ll];_l_=_[(68-0x43)];_l=(992180)while _l_<=(-#[[can someone send me the psu source code it got deletedd]]+(0xfc-155))do _l-= _l _l=(3898335)while(0xff0/204)>=_l_ do _l-= _l _l=(438620)while(2268/0xfc)>=_l_ do _l-= _l _l=(2271250)while(-#'perth thinks psu is bad (it is) and uses ms priv'+(-60+0x70))>=_l_ do _l-= _l _l=(3674405)while(0xaa/170)>=_l_ do _l-= _l _l=(1318618)while _l_>(0x0/151)do _l-= _l __[_[_ll_]]=__[_[____]][_[____l]];break end while 1942==(_l)/((0x581-730))do __[_[___l]]=#__[_[_llll]];break end;break;end while(_l)/((254009/0x83))==1895 do _l=(8867236)while(-#[[i loooove federal]]+(70-(0x8a+-87)))>=_l_ do _l-= _l if(__[_[_l__l]]~=_[____l])then _ll=_ll+_lll;else _ll=_[_llll];end;break;end while 3934==(_l)/((0x93e+-112))do _l=(2578842)while _l_>(0x65-98)do _l-= _l local _=_[___ll]__[_]=__[_](__[_+_lll])break end while(_l)/((-0x15+1920))==1358 do _ll=_[_l__];break end;break;end break;end break;end while(_l)/((0x8fe3f/205))==790 do _l=(8721807)while _l_<=((0x6c-78)+-#"Why are you reading this")do _l-= _l _l=(2176200)while _l_>(-#'how many meme strings do we have'+(-101+0x8a))do _l-= _l __[_[__lll]]=_ll__[_[_l__]];_ll=_ll+__l;_=___[_ll];__[_[_ll_]]=#__[_[_l_l]];_ll=_ll+__l;_=___[_ll];_ll__[_[_l_l]]=__[_[___l]];_ll=_ll+__l;_=___[_ll];__[_[___l]]=_ll__[_[__l_l]];_ll=_ll+__l;_=___[_ll];__[_[__l_]]=#__[_[____]];_ll=_ll+__l;_=___[_ll];_ll__[_[_l__]]=__[_[__lll]];_ll=_ll+__l;_=___[_ll];do return end;break end while(_l)/((3417+-0x45))==650 do __[_[___l]]=__[_[_llll]][__[_[_l_l_]]];break end;break;end while(_l)/((-#"no i legit burned it"+(0x64290/144)))==3083 do _l=(29016)while _l_<=(0x540/192)do _l-= _l if not __[_[___l]]then _ll=_ll+_lll;else _ll=_[_l__];end;break;end while 52==(_l)/((1202-0x284))do _l=(1743360)while _l_>(0x53+-75)do _l-= _l __[_[_ll_]][_[_l__]]=_[____l];break end while 960==(_l)/((0xe67-1871))do __[_[__lll]]=(_[_l_l]~=0);_ll=_ll+_lll;break end;break;end break;end break;end break;end while(_l)/((0x3e3+-31))==455 do _l=(3098216)while(2282/0xa3)>=_l_ do _l-= _l _l=(1850144)while _l_<=(-#[[We all Love Child Porn]]+(-0x6e+143))do _l-= _l _l=(1222452)while _l_>(-#[[helloretard will face off against MoonSec if Federal keeps deleting my strings fuck you]]+(4753/0x31))do _l-= _l local _l_=_[__lll];local ___=_[__ll_];local _l=_l_+2 local _l_={__[_l_](__[_l_+1],__[_l])};for _=1,___ do __[_l+_]=_l_[_];end;local _l_=_l_[1]if _l_ then __[_l]=_l_ _ll=_[_l_l];else _ll=_ll+__l;end;break end while(_l)/((0x1bfc-3600))==343 do _ll__[_[_llll]]=__[_[_ll_]];break end;break;end while(_l)/((537472/(0x214-324)))==716 do _l=(5123760)while(888/0x4a)>=_l_ do _l-= _l if(__[_[_ll_]]==__[_[____l]])then _ll=_ll+_lll;else _ll=_[_llll];end;break;end while 2960==(_l)/((0x208a7/77))do _l=(11003499)while(3172/(583-0x153))<_l_ do _l-= _l __[_[__lll]]=_[_llll];break end while(_l)/((-#'You know lua? name every metamethod - skids of v3rm'+(8328-0x105c)))==2691 do __[_[__l_]]=(_[_l_l]~=0);break end;break;end break;end break;end while 1199==(_l)/((5214-(2756+-0x7e)))do _l=(4890708)while(0x95d/(191+-0x32))>=_l_ do _l-= _l _l=(5327256)while _l_<=(-0x48+87)do _l-= _l if(__[_[___l]]==__[_[_lll_]])then _ll=_ll+_lll;else _ll=_[__l_l];end;break;end while 1496==(_l)/(((631136/0xb0)+-#'1 plus 1 doesnt equal 111'))do _l=(2246630)while((111+-0x5b)+-#"porn")<_l_ do _l-= _l do return end;break end while 1769==(_l)/((0xa6a-1396))do local _l=_[__l_]__[_l](___l_(__,_l+_lll,_[_llll]))break end;break;end break;end while(_l)/(((2757-0x593)+-#"Me when moonsec:"))==3722 do _l=(5108796)while _l_<=(0x6d2/97)do _l-= _l __[_[_ll_]]=__[_[_l_l]][__[_[__llll]]];break;end while 3686==(_l)/((2810-0x590))do _l=(4328390)while _l_>(-#'staymad'+(-0x21+59))do _l-= _l __[_[__lll]]=__[_[_l__]];break end while 3610==(_l)/((0x4641/15))do __[_[_l__l]]={};break end;break;end break;end break;end break;end break;end while 2877==(_l)/((193765/0x8f))do _l=(1289848)while(130-0x63)>=_l_ do _l-= _l _l=(5648104)while _l_<=(-#"Lies"+(0xb7-154))do _l-= _l _l=(7249338)while _l_<=(2728/0x7c)do _l-= _l _l=(929838)while _l_>(0xcb7/155)do _l-= _l _ll=_[____];break end while 338==(_l)/((-#'psu more like psshit hahahaha laugh at my joke everyone'+(-0x3b+2865)))do local _ll=_[_l_l];local _l=__[_ll]for _=_ll+1,_[_lll_]do _l=_l..__[_];end;__[_[__lll]]=_l;break end;break;end while 1971==(_l)/(((7458-0xebd)+-#"staymad"))do _l=(5812101)while _l_<=(0x6b-84)do _l-= _l do return end;break;end while(_l)/((0x1e79-3934))==1503 do _l=(11635610)while _l_>(3408/0x8e)do _l-= _l local _l=_[_l__l];local __l=__[_l]local _l_=__[_l+2];if(_l_>0)then if(__l>__[_l+1])then _ll=_[_ll_l];else __[_l+3]=__l;end elseif(__l<__[_l+1])then _ll=_[_l_l];else __[_l+3]=__l;end break end while(_l)/(((0xfba+-25)+-#"go ahead. replace loadstring with dump. do it."))==2942 do local _l=_[_ll_]__[_l]=__[_l](___l_(__,_l+__l,_[_ll_l]))break end;break;end break;end break;end while 4081==(_l)/(((0x2ce74/131)+-#"no i legit burned it"))do _l=(10329330)while _l_<=(6692/0xef)do _l-= _l _l=(8457328)while(-#"I assure you officer she was a 3000 year old dragon I saw it in those japanese cartoons"+(283-0xaa))>=_l_ do _l-= _l __[_[___ll]][__[_[__l_l]]]=__[_[__ll_]];break;end while 2552==(_l)/((0x1a38-3398))do _l=(11362289)while(94-0x43)<_l_ do _l-= _l local _ll__;local _l_;local _ll_l;local _l;__[_[___ll]]=_l_ll[_[_l__]];_ll=_ll+__l;_=___[_ll];__[_[___l]]=__[_[_l_l]][_[_lll_]];_ll=_ll+__l;_=___[_ll];_l=_[__l_];_ll_l=__[_[____]];__[_l+1]=_ll_l;__[_l]=_ll_l[_[_l_l_]];_ll=_ll+__l;_=___[_ll];__[_[___ll]]=__[_[__l_l]];_ll=_ll+__l;_=___[_ll];__[_[__l_]]=__[_[_l__]];_ll=_ll+__l;_=___[_ll];_l=_[___ll]__[_l]=__[_l](___l_(__,_l+__l,_[_llll]))_ll=_ll+__l;_=___[_ll];_l=_[__lll];_ll_l=__[_[_llll]];__[_l+1]=_ll_l;__[_l]=_ll_l[_[_lll_]];_ll=_ll+__l;_=___[_ll];_l=_[_ll_]__[_l]=__[_l](__[_l+_lll])_ll=_ll+__l;_=___[_ll];_l_={__,_};_l_[_lll][_l_[__ll][___ll]]=_l_[__l][_l_[__ll][____l]]+_l_[_lll][_l_[__ll][_llll]];_ll=_ll+__l;_=___[_ll];__[_[__l_]]=__[_[_l_l]]%_[____l];_ll=_ll+__l;_=___[_ll];_l=_[_ll_]__[_l]=__[_l](__[_l+_lll])_ll=_ll+__l;_=___[_ll];_ll_l=_[____];_ll__=__[_ll_l]for _=_ll_l+1,_[_l___]do _ll__=_ll__..__[_];end;__[_[_l__l]]=_ll__;_ll=_ll+__l;_=___[_ll];_l_={__,_};_l_[_lll][_l_[__ll][___l]]=_l_[__l][_l_[__ll][_l___]]+_l_[_lll][_l_[__ll][_l__]];_ll=_ll+__l;_=___[_ll];__[_[__l_]]=__[_[_l_l]]%_[__ll_];break end while 2857==(_l)/((-116+0xffd))do local _l=_[_ll_];local _l_=__[_l+2];local __l=__[_l]+_l_;__[_l]=__l;if(_l_>0)then if(__l<=__[_l+1])then _ll=_[_l__];__[_l+3]=__l;end elseif(__l>=__[_l+1])then _ll=_[_l_l];__[_l+3]=__l;end break end;break;end break;end while 3390==(_l)/(((0x99076/101)-3159))do _l=(1723700)while(((-74+0x168)-0xcc)+-#'Day 2 of telling federal that he spilled out his milk')>=_l_ do _l-= _l __[_[___l]]=__[_[_ll_l]][_[____l]];break;end while(_l)/((0x461+-21))==1567 do _l=(1543968)while(76-0x2e)<_l_ do _l-= _l if(__[_[___ll]]~=__[_[_l_l_]])then _ll=_ll+_lll;else _ll=_[_l_l];end;break end while 864==(_l)/((0x711+-22))do local _l=_[_ll_];local _l_=__[_l+2];local __l=__[_l]+_l_;__[_l]=__l;if(_l_>0)then if(__l<=__[_l+1])then _ll=_[_l__];__[_l+3]=__l;end elseif(__l>=__[_l+1])then _ll=_[____];__[_l+3]=__l;end break end;break;end break;end break;end break;end while(_l)/((0x39c-490))==2972 do _l=(176750)while(-#'powered by ROBLOX Corporation'+(0x32c8/200))>=_l_ do _l-= _l _l=(10018504)while(0x1e09/233)>=_l_ do _l-= _l _l=(3381722)while _l_>(98-0x42)do _l-= _l local _ll=_[_ll_];local _l=__[_[_llll]];__[_ll+1]=_l;__[_ll]=_l[_[_l_l_]];break end while 1973==(_l)/((0xdb1-1791))do _l_ll[_[____]]=__[_[__l_]];break end;break;end while 2504==(_l)/((-#'still cant find the cum?'+(-37+0xfde)))do _l=(31158)while _l_<=(4080/0x78)do _l-= _l __[_[___l]]=__[_[____]]%_[_lll_];break;end while 54==(_l)/(((1413-0x302)+-#"This file has been enchanted with uncrackable V, fuck the fuck off"))do _l=(4834860)while(161+-0x7e)<_l_ do _l-= _l __[_[_ll_]]={};break end while 1220==(_l)/((7942-0xf8b))do local _=_[_ll_]__[_](__[_+_lll])break end;break;end break;end break;end while 350==(_l)/((-0x72+619))do _l=(683774)while(-#'do you ever shut the fuck up perth'+(167+-0x5e))>=_l_ do _l-= _l _l=(1026025)while _l_<=(-#":)))))))"+((-0xb2+80)+143))do _l-= _l __[_[___ll]]=__[_[__l_l]]-__[_[_lll_]];break;end while 275==(_l)/(((347576/0x5c)+-#[[KFC tried to justify urls as fake constants LOL]]))do _l=(14274)while _l_>(-0x4d+115)do _l-= _l __[_[_ll_]]=__[_[____]]%_[_l_l_];break end while 26==(_l)/((-0x3b+608))do local _l;local _l_;local __ll,___l;local _l_l;local _l;__[_[_ll_]]=_l_ll[_[____]];_ll=_ll+__l;_=___[_ll];__[_[_ll_]]=__[_[__l_l]][_[_l___]];_ll=_ll+__l;_=___[_ll];__[_[_l__l]]=__[_[_ll_l]][_[_lll_]];_ll=_ll+__l;_=___[_ll];__[_[__lll]]=__[_[_ll_l]][_[____l]];_ll=_ll+__l;_=___[_ll];_l=_[__lll];_l_l=__[_[____]];__[_l+1]=_l_l;__[_l]=_l_l[_[_lll_]];_ll=_ll+__l;_=___[_ll];_l=_[__l_]__ll,___l=___lll(__[_l](__[_l+_lll]))__l__=___l+_l-__l _l_=0;for _=_l,__l__ do _l_=_l_+__l;__[_]=__ll[_l_];end;_ll=_ll+__l;_=___[_ll];_l=_[__l_]__ll={__[_l](___l_(__,_l+1,__l__))};_l_=0;for _=_l,_[__llll]do _l_=_l_+__l;__[_]=__ll[_l_];end _ll=_ll+__l;_=___[_ll];_ll=_[_l__];break end;break;end break;end while 1183==(_l)/((626+-0x30))do _l=(5113196)while _l_<=(-#[[perth is an illusion by perth to hide perth from perth]]+(0xf1-147))do _l-= _l local _=_[___l]__[_]=__[_](__[_+_lll])break;end while(_l)/((-#'bald'+(0xbd2-(-75+0x65a))))==3476 do _l=(310878)while(8036/0xc4)<_l_ do _l-= _l local _l_;local _l;__[_[___l]]=__[_[__l_l]][_[_l_l_]];_ll=_ll+__l;_=___[_ll];__[_[__l_]]=__[_[_l_l]][_[_l___]];_ll=_ll+__l;_=___[_ll];__[_[__lll]]=_l_ll[_[__l_l]];_ll=_ll+__l;_=___[_ll];__[_[__lll]]=__[_[_llll]][_[__llll]];_ll=_ll+__l;_=___[_ll];__[_[___l]]=__[_[_ll_l]][_[_l_l_]];_ll=_ll+__l;_=___[_ll];__[_[__l_]]=__[_[_l__]][_[____l]];_ll=_ll+__l;_=___[_ll];__[_[_ll_]]=__[_[____]][__[_[__ll_]]];_ll=_ll+__l;_=___[_ll];__[_[___ll]][_[_ll_l]]=__[_[_l___]];_ll=_ll+__l;_=___[_ll];_l=_[___ll];_l_=__[_[_l_l]];__[_l+1]=_l_;__[_l]=_l_[_[_l___]];_ll=_ll+__l;_=___[_ll];_l=_[___l]__[_l](__[_l+_lll])_ll=_ll+__l;_=___[_ll];_l=_[__lll];_l_=__[_[_l__]];__[_l+1]=_l_;__[_l]=_l_[_[____l]];_ll=_ll+__l;_=___[_ll];_l=_[_ll_]__[_l](__[_l+_lll])_ll=_ll+__l;_=___[_ll];__[_[_l__l]]=_l_ll[_[_ll_l]];_ll=_ll+__l;_=___[_ll];__[_[___l]]();_ll=_ll+__l;_=___[_ll];__[_[___l]]=_l_ll[_[_ll_l]];_ll=_ll+__l;_=___[_ll];__[_[__l_]]=__[_[_llll]][_[____l]];_ll=_ll+__l;_=___[_ll];__[_[___l]]=__[_[__l_l]][_[__ll_]];_ll=_ll+__l;_=___[_ll];__[_[___l]]=__[_[____]][_[_lll_]];_ll=_ll+__l;_=___[_ll];__[_[___ll]][_[____]]=__[_[__ll_]];break end while(_l)/((767-0x1a9))==909 do __[_[__lll]]=(_[_l_l]~=0);break end;break;end break;end break;end break;end break;end break;end while 3730==(_l)/((659-(833-0x1b8)))do _l=(2812140)while _l_<=(-#[[water is wet]]+(-0x62+173))do _l-= _l _l=(6822225)while _l_<=((0xaf+-104)+-#'Jeff Bezos approved')do _l-= _l _l=(796536)while _l_<=(0x92+-99)do _l-= _l _l=(28116)while((-77+0x89)+-#"Federal is godly")>=_l_ do _l-= _l _l=(3427272)while(0x9c-113)<_l_ do _l-= _l __[_[__l_]]=__[_[_llll]];break end while(_l)/((0xc02d6/226))==984 do local _l=_[__l_];local _ll=__[_[__l_l]];__[_l+1]=_ll;__[_l]=_ll[_[__ll_]];break end;break;end while(_l)/((0x73+-82))==852 do _l=(4118828)while _l_<=((28305/0xff)+-#'This file has been enchanted with uncrackable V, fuck the fuck off')do _l-= _l __[_[___l]]=_____(_lllll[_[__l_l]],nil,_l_ll);break;end while(_l)/(((-0x4cc8/156)+1144))==4046 do _l=(9898879)while _l_>(5520/0x78)do _l-= _l __[_[_ll_]][_[_ll_l]]=__[_[__ll_]];break end while(_l)/((0xac5b8/232))==3253 do if(__[_[__lll]]~=_[__ll_])then _ll=_ll+_lll;else _ll=_[_l_l];end;break end;break;end break;end break;end while 2664==(_l)/(((0x6f94/74)+-#'helloretard will face off against MoonSec if Federal keeps deleting my strings fuck you'))do _l=(1864464)while(-#"hint: the script is in line 1"+((-#[[This file has been enchanted with uncrackable V, fuck the fuck off]]+(0x13b+-55))-0x74))>=_l_ do _l-= _l _l=(13630335)while _l_>((23814/0xf3)+-#'Do you even know what sizeof size_t equals to Lmao')do _l-= _l __[_[_l__l]][_[_ll_l]]=__[_[__llll]];break end while 3715==(_l)/((418266/(7866/0x45)))do _ll__[_[_ll_l]]=__[_[__l_]];break end;break;end while(_l)/((-#'Lies'+(5315-0xa93)))==716 do _l=(4898775)while(-88+(0xad+-35))>=_l_ do _l-= _l __[_[__l_]][_[_llll]]=_[____l];break;end while 3225==(_l)/((3092-(-#"The Great Sage Equal To Heaven is here Luraph users hide!!!!"+(0x33080/128))))do _l=(3178092)while(0xb3-128)<_l_ do _l-= _l local _={__,_};_[_lll][_[__ll][__l_]]=_[__l][_[__ll][____l]]+_[_lll][_[__ll][_l_l]];break end while 2014==(_l)/((-0x5c+1670))do local __ll=_lllll[_[_l_l]];local _l_;local _l={};_l_=_lll_l({},{__index=function(__,_)local _=_l[_];return _[1][_[2]];end,__newindex=function(_ll,_,__)local _=_l[_]_[1][_[2]]=__;end;});for __l=1,_[__ll_]do _ll=_ll+_lll;local _=___[_ll];if _[((0xf2-181)+-#'The Great Sage Equal To Heaven is here Luraph users hide!!!!')]==44 then _l[__l-1]={__,_[_ll_l]};else _l[__l-1]={_ll__,_[_l__]};end;_l_lll[#_l_lll+1]=_l;end;__[_[__lll]]=_____(__ll,_l_,_l_ll);break end;break;end break;end break;end break;end while 2025==(_l)/((0x1a95-3436))do _l=(1237712)while _l_<=(8094/0x8e)do _l-= _l _l=(1013424)while(179+-0x7d)>=_l_ do _l-= _l _l=(109720)while(10759/0xcb)<_l_ do _l-= _l _l_ll[_[_l__]]=__[_[_ll_]];_ll=_ll+__l;_=___[_ll];__[_[___ll]]={};_ll=_ll+__l;_=___[_ll];__[_[__lll]]={};_ll=_ll+__l;_=___[_ll];_l_ll[_[_llll]]=__[_[___l]];_ll=_ll+__l;_=___[_ll];__[_[_l__l]]=_l_ll[_[_llll]];_ll=_ll+__l;_=___[_ll];if(__[_[__l_]]~=_[_l___])then _ll=_ll+_lll;else _ll=_[_l_l];end;break end while(_l)/((-83+0x25b))==211 do local _l_;local _l;_l_ll[_[__l_l]]=__[_[__lll]];_ll=_ll+__l;_=___[_ll];__[_[_ll_]]=_l_ll[_[__l_l]];_ll=_ll+__l;_=___[_ll];__[_[___l]]=_[____];_ll=_ll+__l;_=___[_ll];_l=_[__l_]__[_l](__[_l+_lll])_ll=_ll+__l;_=___[_ll];__[_[___ll]]=_l_ll[_[_llll]];_ll=_ll+__l;_=___[_ll];__[_[___ll]][_[_l_l]]=_[_l_l_];_ll=_ll+__l;_=___[_ll];__[_[__lll]]=_l_ll[_[____]];_ll=_ll+__l;_=___[_ll];_l=_[_l__l];_l_=__[_[____]];__[_l+1]=_l_;__[_l]=_l_[_[____l]];_ll=_ll+__l;_=___[_ll];__[_[___l]]=_[_ll_l];_ll=_ll+__l;_=___[_ll];_l=_[_l__l]__[_l]=__[_l](___l_(__,_l+__l,_[__l_l]))break end;break;end while 258==(_l)/((-0x29+(3991+-0x16)))do _l=(6342224)while _l_<=(5060/0x5c)do _l-= _l __[_[_l__l]]=_____(_lllll[_[_l_l]],nil,_l_ll);break;end while(_l)/((-85+0xd58))==1904 do _l=(6351165)while((206-0x8f)+-#"hi skid")<_l_ do _l-= _l local _={__,_};_[_lll][_[__ll][__lll]]=_[__l][_[__ll][_lll_]]+_[_lll][_[__ll][____]];break end while(_l)/((0x6cdc5/119))==1695 do __[_[___ll]]=_l_ll[_[____]];break end;break;end break;end break;end while 688==(_l)/((0xe38-1841))do _l=(7434049)while(0x3480/224)>=_l_ do _l-= _l _l=(1101493)while(0xa6+-108)>=_l_ do _l-= _l _l_ll[_[_l__]]=__[_[_l__l]];break;end while(_l)/((-0x5b+668))==1909 do _l=(548064)while(0xc8-141)<_l_ do _l-= _l if __[_[_ll_]]then _ll=_ll+__l;else _ll=_[_l_l];end;break end while(_l)/(((0x190d-3230)-0x65a))==352 do __[_[_l__l]]();break end;break;end break;end while 2443==(_l)/((-108+0xc4f))do _l=(13792680)while _l_<=(175+-0x72)do _l-= _l local _=_[__l_]local _ll,_l=___lll(__[_](__[_+_lll]))__l__=_l+_-__l local _l=0;for _=_,__l__ do _l=_l+__l;__[_]=_ll[_l];end;break;end while 3870==(_l)/((-#"ligma balls"+(0x1c67-3696)))do _l=(10311588)while _l_>(-#"teefus more like pedofus"+(201-0x73))do _l-= _l if not __[_[_ll_]]then _ll=_ll+_lll;else _ll=_[_l_l];end;break end while(_l)/((555768/0xba))==3451 do local _lll;local _l_;local _l;__[_[__lll]]=_[_l__];_ll=_ll+__l;_=___[_ll];__[_[___ll]]=_[_ll_l];_ll=_ll+__l;_=___[_ll];__[_[___ll]]=#__[_[_l_l]];_ll=_ll+__l;_=___[_ll];__[_[__l_]]=_[_llll];_ll=_ll+__l;_=___[_ll];_l=_[___l];_l_=__[_l]_lll=__[_l+2];if(_lll>0)then if(_l_>__[_l+1])then _ll=_[__l_l];else __[_l+3]=_l_;end elseif(_l_<__[_l+1])then _ll=_[__l_l];else __[_l+3]=_l_;end break end;break;end break;end break;end break;end break;end while(_l)/((0xb715/51))==3060 do _l=(8640834)while _l_<=(0x87+-61)do _l-= _l _l=(2733159)while(157-0x59)>=_l_ do _l-= _l _l=(5976740)while _l_<=((-48+0x97)+-#'Broo u/thatHEXdude slapped this server')do _l-= _l _l=(6576534)while(-119+0xb7)<_l_ do _l-= _l __[_[__l_]]=_ll__[_[_ll_l]];break end while(_l)/((-0x47+2564))==2638 do __[_[_l__l]]=_[____];break end;break;end while(_l)/((0x630+-44))==3881 do _l=(1593558)while _l_<=(-#"someone play kogama with perth please hes so lonely"+(303-0xba))do _l-= _l local _l_=_lllll[_[_llll]];local __l;local _l={};__l=_lll_l({},{__index=function(__,_)local _=_l[_];return _[1][_[2]];end,__newindex=function(_ll,_,__)local _=_l[_]_[1][_[2]]=__;end;});for __l=1,_[__llll]do _ll=_ll+_lll;local _=___[_ll];if _[(0x66-101)]==44 then _l[__l-1]={__,_[_llll]};else _l[__l-1]={_ll__,_[_l__]};end;_l_lll[#_l_lll+1]=_l;end;__[_[__l_]]=_____(_l_,__l,_l_ll);break;end while(_l)/(((2526-0x515)+-#'oh wait thats an invalid character'))==1338 do _l=(10682208)while _l_>(-#[[This file has been enchanted with uncrackable V, fuck the fuck off]]+(-25+0x9e))do _l-= _l local _l=_[__l_]local _l_={__[_l](___l_(__,_l+1,__l__))};local _ll=0;for _=_l,_[__ll_]do _ll=_ll+__l;__[_]=_l_[_ll];end break end while(_l)/(((-#'while true do end'+(0x12fca0/220))-2855))==3837 do __[_[___l]][__[_[_l_l]]]=__[_[_l_l_]];break end;break;end break;end break;end while 3289==(_l)/(((0x4b320/176)-919))do _l=(1387161)while _l_<=((128+-0x2d)+-#"i love perth")do _l-= _l _l=(6943)while _l_<=((17808/0x70)+-#'I have enchanted this script with uncrackable V, your only option is to fuck the fuck off.')do _l-= _l __[_[___l]]();break;end while 131==(_l)/(((5994/0x51)+-#"Shard fard poo gaymer"))do _l=(607848)while _l_>((23760/0xa5)+-#[[Arse Bloody Bugger Cow Crap Damn Ginger Git God Goddam Jesus Christ Minger]])do _l-= _l if(__[_[_ll_]]~=__[_[__llll]])then _ll=_ll+_lll;else _ll=_[_l_l];end;break end while(_l)/((339+-0x51))==2356 do local _l=_[_l__l];local __l=__[_l]local _l_=__[_l+2];if(_l_>0)then if(__l>__[_l+1])then _ll=_[_l__];else __[_l+3]=__l;end elseif(__l<__[_l+1])then _ll=_[_l_l];else __[_l+3]=__l;end break end;break;end break;end while 1951==(_l)/((1521-0x32a))do _l=(621432)while(-66+0x8a)>=_l_ do _l-= _l __[_[_ll_]]=#__[_[_l_l]];break;end while(_l)/((18900/0x4b))==2466 do _l=(4395309)while _l_>(224-0x97)do _l-= _l local _=_[_ll_]local _ll,_l=___lll(__[_](__[_+_lll]))__l__=_l+_-__l local _l=0;for _=_,__l__ do _l=_l+__l;__[_]=_ll[_l];end;break end while(_l)/(((-91+0x701)+-#"<@!761654159095103499> shut the fuck up"))==2643 do local _l_=_[___ll];local ___=_[_l_l_];local _l=_l_+2 local _l_={__[_l_](__[_l_+1],__[_l])};for _=1,___ do __[_l+_]=_l_[_];end;local _l_=_l_[1]if _l_ then __[_l]=_l_ _ll=_[_llll];else _ll=_ll+__l;end;break end;break;end break;end break;end break;end while 3414==(_l)/(((332085/0x83)+-#[[Nigh]]))do _l=(2042838)while(-0x12+97)>=_l_ do _l-= _l _l=(2099776)while(138+-0x3e)>=_l_ do _l-= _l _l=(1223334)while(-48+0x7b)<_l_ do _l-= _l local _l=_[___ll]local _l_={__[_l](___l_(__,_l+1,__l__))};local _ll=0;for _=_l,_[_lll_]do _ll=_ll+__l;__[_]=_l_[_ll];end break end while 1387==(_l)/((-#'midruto'+(-25+0x392)))do if __[_[___l]]then _ll=_ll+__l;else _ll=_[_l_l];end;break end;break;end while(_l)/((0x532-728))==3488 do _l=(3518655)while _l_<=((0x83+-19)+-#[[stop looking at me im showering smh]])do _l-= _l __[_[_ll_]]=_l_ll[_[_ll_l]];break;end while(_l)/((-#[[How to dump moonsec]]+(-0x57+2521)))==1457 do _l=(8325747)while(16380/0xd2)<_l_ do _l-= _l local _=_[__l_]__[_](__[_+_lll])break end while 2943==(_l)/(((0x16b3-(-#'POV New owners'+(596000/0xc8)))+-#"follow your nose"))do local _l=_[_l__l]__[_l](___l_(__,_l+_lll,_[_l__]))break end;break;end break;end break;end while(_l)/(((-23+0x25a)+-#'Shard fard poo gaymer'))==3661 do _l=(6721814)while(0xf9-167)>=_l_ do _l-= _l _l=(9540784)while _l_<=(-0x78+200)do _l-= _l do return __[_[_l__l]]end break;end while(_l)/(((0x6b637/151)+-#'This script was obfuscated with luasecure'))==3322 do _l=(7014540)while _l_>(0x103-178)do _l-= _l local _l=_[_ll_]__[_l]=__[_l](___l_(__,_l+__l,_[____]))break end while(_l)/(((6449-0xcc4)+-#"True af"))==2210 do __[_[___l]]=__[_[_ll_l]]-__[_[____l]];break end;break;end break;end while(_l)/((1984+(-#"Ok federal give us MSv3 when"+(306/0x99))))==3433 do _l=(11983344)while(0xd2+-127)>=_l_ do _l-= _l local _ll=_[_l__];local _l=__[_ll]for _=_ll+1,_[_lll_]do _l=_l..__[_];end;__[_[___l]]=_l;break;end while(_l)/((-#'Searching for the wrapper function'+(0x6bf94/130)))==3558 do _l=(129066)while _l_>(-#'win+L = solution'+(-78+0xb2))do _l-= _l do return __[_[___l]]end break end while(_l)/((0xa1ee/141))==439 do __[_[__l_]]=(_[____]~=0);_ll=_ll+_lll;break end;break;end break;end break;end break;end break;end break;end _ll+= _lll end;end);end;return _____(_ll_ll(),{},__l__l())()end)_msec({[(245+-0x43)]='\115\116'..(function(_)return(_ and'㒘㒠㒝㒛㒣㒘㒣㒣㒦㒦㒦')or'\114\105'or'\120\58'end)((-118+(10947/0x59))==(-0x17+29))..'\110g',["㒤㒥㒞㒛㒚㒚㒥㒙㒚㒥"]='\108\100'..(function(_)return(_ and'㒥㒥㒠㒥㒡㒡㒝㒦㒚㒣㒠㒜㒣㒠㒦㒞㒛㒣')or'\101\120'or'\119\111'end)((0x5f+-90)==(-#'big harry black guy nuts'+(-0x46+100)))..'\112',["㒘㒚㒢㒘㒛㒗㒗㒛㒛"]=(function(_)return(_ and'㒦㒟㒗㒤㒞㒦㒝㒣㒥㒢㒤㒛㒤㒙')and'\98\121'or'\100\120'end)((1265/0xfd)==(128+-0x7b))..'\116\101',["㒝㒡㒞㒤㒜㒤㒚㒜㒝㒡㒡㒥㒞㒥㒙㒤"]='\99'..(function(_)return(_ and'㒟㒚㒣㒤㒙㒘㒟㒗㒥㒛㒦㒞㒘')and'\90\19\157'or'\104\97'end)((-94+0x63)==(0x2d-42))..'\114',[(-0x5c+681)]='\116\97'..(function(_)return(_ and'㒢㒥㒟㒘㒥㒡㒚㒛㒙㒦㒟㒗㒟㒠')and'\64\113'or'\98\108'end)(((0x30-36)+-#[[hacker]])==(0x46/14))..'\101',["㒘㒥㒛㒥㒛㒘㒝㒛"]=(function(_)return(_ and'㒜㒛㒛㒛㒢㒝㒜㒢㒠㒦㒜㒦㒥')or'\115\117'or'\78\107'end)((0x64-97)==(0x5b-60))..'\98',["㒛㒙㒗㒛㒝㒠㒞㒢㒞㒛㒢㒠㒡㒜"]='\99\111'..(function(_)return(_ and'㒛㒝㒗㒟㒛㒤㒦㒚㒥㒣㒡㒚㒣㒤㒙㒗㒤')and'\110\99'or'\110\105\103\97'end)((0x78+(-#'// rip gmod users'+(-15768/0xdb)))==(-#[[perth is an illusion by perth to hide perth from perth]]+(133+-0x30)))..'\97\116',[((2869760/0x26)/0x76)]=(function(_,_l)return(_ and'㒡㒥㒤㒙㒜㒘㒘㒗㒚㒠㒥㒦㒚㒝㒙㒢㒡㒡㒗')and'\48\159\158\188\10'or'\109\97'end)((102-0x61)==(47-0x29))..'\116\104',[(((-0x2e+293178)/0xcb)+-#[[psst.. change all returns to dump to get the source code]])]=(function(_,_l)return((31-(0x93+-121))==(453/0x97)and'\48'..'\195'or _..((not'\20\95\69'and'\90'..'\180'or _l)))or'\199\203\95'end),["㒟㒛㒙㒙㒢㒜㒦㒛㒛㒚"]='\105\110'..(function(_,_l)return(_ and'㒗㒚㒠㒘㒛㒡㒢㒗㒗㒡㒥㒗㒙㒝㒤㒜㒡㒝㒤')and'\90\115\138\115\15'or'\115\101'end)((-#"oh, i forgot i can write some shit here so ya dummies will see it"+(0x31c4/182))==(0x59-58))..'\114\116',["㒦㒝㒝㒦㒘㒚㒣㒞㒡"]='\117\110'..(function(_,_l)return(_ and'㒞㒡㒞㒝㒣㒞㒣㒝㒗㒠㒗㒝㒞')or'\112\97'or'\20\38\154'end)((480/0x60)==(0x60-65))..'\99\107',["㒟㒡㒗㒣㒤㒞㒢㒞㒠㒡㒘"]='\115\101'..(function(_)return(_ and'㒝㒦㒜㒡㒡㒟㒝㒙㒡㒥㒙㒥')and'\110\112\99\104'or'\108\101'end)((0x46-65)==(2046/0x42))..'\99\116',["㒟㒛㒚㒙㒢㒦㒗㒢㒞㒥㒥㒦"]='\116\111\110'..(function(_,_l)return(_ and'㒦㒘㒥㒘㒦㒥㒛㒙㒢㒦㒜㒞㒞㒢㒝㒘')and'\117\109\98'or'\100\97\120\122'end)((-#[[control c, control v]]+(((6400+-0x12)+-#'Oh so you know C++? What does sizeof(int) equal to? (gcc)')/253))==((-0x20+77)+-#'Found an xxxxxxxxxl store for ur fat mom'))..'\101\114'},{["㒞㒙㒡㒣㒞㒙㒢㒞㒡㒗㒤㒥㒝㒞"]=((getfenv))},((getfenv))()) end)()
        end)
    
        BullySection:NewButton("Ki Spam", "Press V to spam", function()
            Move1 = "Sudden Storm"
    Move2 = "Finish Breaker"
    Move3 = "Demon Flash"
    Move4 = "Big Bang Kamehameha"
    Move5 = "Burning Blast"
    Move6 = "Justice Flash"
    Move7 = "Divine Lasso"
    Move8 = "Pressure Gauge"
    Move9 = "Blaster Meteor"
    --
    MSKey = "v" -- Change the key inside the quotations to whatever key you want to use to toggle your movespam.
    --
    _cMhlNnFWdeO1FLGW, Protected_by_MoonSecV2, Discord = 'discord.gg/gQEH2uZxUk'
    ,nil,nil;(function() _msec=(function(_,_l,__)local __l__l=_l["㒞㒙㒡㒣㒞㒙㒢㒞㒡㒗㒤㒥㒝㒞"];local _ll__l=__[_[(-#{'nil';(function()return{','}end)(),1,'}',(function()return#{('pFFFbm'):find("\70")}>0 and 1 or 0 end)}+645)]][_["㒤㒥㒞㒛㒚㒚㒥㒙㒚㒥"]];local __ll=(0x46-66)/(0x49+(-#[[im dying]]+((-8+-0x2c)-11)))local _lll=((0xa1+(-0xbc1/51))+-0x64)-(38-0x25)local ___lll=__[_[(0x1bb-265)]][_["㒘㒚㒢㒘㒛㒗㒗㒛㒛"]];local __l__=(((0x171+((-167+0x32)+-#[[Fuck]]))-169)+-0x4e)+(44+-0x2a)local _l_ll=__[_[(596+-#{",",85;'}';'nil';(function()return{','}end)(),150,'}'})]][_["㒛㒙㒗㒛㒝㒠㒞㒢㒞㒛㒢㒠㒡㒜"]]local __l=((0x12a1/251)+-#'free nitro real?!')-((0x7d+(-25+((-78+0xb)+-#[[cock and ball]])))+-#[[happy birdday wally]])local ____l=((((4080+-#{(function()return{','}end)();'nil',(function()return#{('fpPfll'):find("\80")}>0 and 1 or 0 end)})/27)+-#"deobfuscation in progress")+-0x7a)local _lll_=((((0x22d-(313+-#{(function()return{','}end)(),30;{};'nil',{},1;","}))+-#'This code was obfuscated using PSU, which stands for Penis Sucking Utilities')-106)+-#'guys i am epic hackerman i just converted a script to string.byte')local _l___=(-#[[am gay]]+(-0x7d+(0xea+((-#'How to dump moonsec'+(-0x343f7a/234))/0x94))))local __llll=((-#{'}';",",133;",";",",(function()return#{('BHbkpP'):find("\98")}>0 and 1 or 0 end)}+69)+-0x3b)local _l_l_=((-104-((-0xd12+-42)/0x9a))+86)local __ll_=(((-0x5b+((601+-0x59)-0x117))+-#[[_Ben is godly]])-125)local __lll=(0xc8/((325+-#{{},79;79;(function()return{','}end)(),25;79})-219))local ___l=(6+-#{1,",";(function()return{','}end)(),1})local _l__l=(63+(-#"bit.bdiv(0,0)"+((89-(249-((-94+0x122)+-#[[obfuscator tooooo gooood]])))-60)))local _ll_=(-#'are you maybe is the or the maybe is the or the maybe hm'+(((-0x5348/(513-(0x167+-51)))-3)+165))local ___ll=((-59+(0x12e+((-124+0x2c)+-#'FREE LUA OBFUSCATOR DOWNLOAD REAL NO FAKE 2024')))+-115)local __l_=(432/((54145/(58310/(-#[[string]]+(0x346c/55))))+-#'troll'))local __l_l=((-90+(147+-#{'}',{},1;(function()return{','}end)();104,{};(function()return#{('BFmHoP'):find("\109")}>0 and 1 or 0 end)}))+-#'psst constant table just below this meme string')local _l_l=((((-0xd26d+26905)/0x7e)+0x57)+130)local ____=(-#{",";{};(function()return{','}end)()}+6)local _l__=((100+-#{'nil',",";",",1,1})+-0x5c)local _llll=(9+-#{(function()return{','}end)(),73;95,95,73;","})local _ll_l=((144-((1789+-#{",",60;168;60})/15))+-#"what the fuck is sleep")local __ll_l=_[(1394+-#{'}',{};'}','nil';1,86})];local _l_l_l=__[_[(185+-#{(function()return{','}end)(),'}';{};131,1,54,'nil'})]][_["㒘㒥㒛㒥㒛㒘㒝㒛"]];local _lll_l=__[(function(_)return type(_):sub(1,1)..'\101\116'end)('㒝㒣㒦㒠㒘㒤㒘㒠')..'\109\101'..('\116\97'or'㒞㒘㒘㒝㒦㒙㒡㒞').._[((-0x39-28)+0x2a2)]];local __l_ll=__[_[(1245-0x290)]][_["㒟㒛㒙㒙㒢㒜㒦㒛㒛㒚"]];local _lllll=(186/0x5d)-(50-(-#'this file has been secured with a wall the size of your mother'+((0x2102/26)-215)))local _____=(-0x2e+((193+(-119+0x23))+-#[[psu got dumped so hard their entire source code came out rofl]]))-(-86+0x58)local _l__ll=__[_[(184+-#{'}',",";'}';{};'}';{}})]][_["㒝㒡㒞㒤㒜㒤㒚㒜㒝㒡㒡㒥㒞㒥㒙㒤"]];local _l=function(_l,_)return _l.._ end local _l_lll=(0x3f-59)*(57+((-0x31-((-0x35+68)+-#[[Why are you reading this]]))+-#"constant dumB"))local ____ll=__[_["㒟㒡㒗㒣㒤㒞㒢㒞㒠㒡㒘"]];local ___=(0x28/20)*(25216/((9547014/0xf6)/0xc5))local _ll_ll=((-0x55+104533)/0x66)*((128-((-204+0x56)+0xcb))+-#"oh oh i will hack you =opens dev console=")local ___l_l=(0x90-(-#[[is it me or everyones feeling like ghostpinging <@!519139355118534656> ?]]+(-84+(0x23a-322))))local _ll__=(-#[[are you maybe is the or the maybe is the or the maybe hm]]+(((-109+0x16)+253)-0x6c))*(-#[[i dont care that this was enchanted with uncrackable V]]+(134-0x4e))local ___l_=__[_["㒦㒝㒝㒦㒘㒚㒣㒞㒡"]]or __[_[((1284-0x2a6)+-#[[while true do end]])]][_["㒦㒝㒝㒦㒘㒚㒣㒞㒡"]];local _l_=(((2489-0x514)-0x27f)-294)local _=__[_["㒟㒛㒚㒙㒢㒦㒗㒢㒞㒥㒥㒦"]];local __l_ll=(function(_l_)local ___,__=3,0x10 local _l={j={},v={}}local _ll=-__l local _=__+_lll while true do _l[_l_:sub(_,(function()_=___+_ return _-_lll end)())]=(function()_ll=_ll+__l return _ll end)()if _ll==(_l_lll-__l)then _ll=""__=_lllll break end end local _ll=#_l_ while _<_ll+_lll do _l.v[__]=_l_:sub(_,(function()_=___+_ return _-_lll end)())__=__+__l if __%__ll==_lllll then __=_____ __l_ll(_l.j,(_l__ll((_l[_l.v[_____]]*_l_lll)+_l[_l.v[__l]])))end end return _l_ll(_l.j)end)("..:::MoonSec::..㒗㒘㒙㒚㒛㒜㒝㒞㒟㒠㒡㒢㒣㒤㒥㒦㒦㒣㒛㒞㒦㒞㒡㒞㒙㒦㒘㒗㒢㒞㒝㒞㒘㒞㒗㒡㒤㒦㒟㒟㒛㒠㒥㒟㒠㒡㒜㒢㒦㒣㒢㒠㒦㒟㒢㒗㒜㒞㒗㒞㒢㒞㒤㒥㒟㒝㒚㒠㒥㒙㒠㒡㒛㒞㒥㒟㒠㒡㒛㒣㒠㒟㒜㒘㒦㒞㒡㒞㒜㒞㒛㒤㒙㒗㒤㒠㒞㒣㒘㒡㒤㒣㒠㒠㒛㒤㒥㒣㒡㒠㒥㒟㒡㒗㒛㒞㒦㒞㒡㒞㒡㒥㒝㒟㒙㒚㒤㒙㒟㒡㒚㒞㒤㒣㒟㒣㒚㒢㒢㒚㒛㒚㒥㒞㒠㒞㒛㒞㒛㒢㒘㒠㒣㒗㒝㒥㒘㒥㒣㒣㒟㒠㒗㒣㒥㒤㒟㒣㒛㒜㒦㒢㒢㒠㒦㒗㒠㒞㒛㒞㒦㒞㒦㒞㒣㒚㒝㒟㒚㒗㒣㒣㒟㒠㒗㒥㒥㒣㒠㒗㒜㒠㒟㒣㒚㒞㒥㒞㒠㒞㒟㒤㒝㒝㒘㒠㒢㒡㒝㒣㒚㒠㒝㒣㒘㒞㒣㒞㒞㒞㒝㒡㒚㒦㒥㒣㒡㒡㒜㒢㒘㒠㒛㒠㒦㒞㒡㒞㒜㒞㒝㒝㒦㒥㒥㒠㒙㒘㒣㒞㒞㒞㒙㒞㒘㒥㒥㒣㒡㒢㒚㒡㒦㒣㒢㒠㒝㒤㒘㒗㒢㒡㒝㒣㒚㒠㒝㒤㒘㒞㒣㒞㒞㒞㒞㒞㒛㒚㒥㒟㒢㒗㒛㒣㒗㒠㒛㒟㒦㒦㒡㒞㒜㒞㒗㒞㒦㒦㒤㒢㒟㒢㒚㒞㒣㒞㒠㒝㒛㒡㒦㒢㒗㒦㒦㒘㒠㒞㒛㒞㒦㒞㒗㒝㒢㒝㒞㒡㒘㒣㒣㒡㒟㒣㒚㒠㒤㒣㒟㒣㒛㒟㒚㒛㒚㒡㒥㒞㒠㒞㒛㒞㒛㒚㒗㒣㒢㒥㒗㒟㒢㒣㒝㒞㒘㒞㒣㒞㒢㒡㒠㒚㒛㒝㒦㒥㒡㒜㒘㒚㒡㒗㒛㒞㒦㒞㒡㒞㒢㒥㒝㒟㒙㒛㒣㒣㒟㒡㒙㒣㒥㒜㒠㒡㒚㒣㒤㒥㒛㒙㒥㒞㒠㒞㒛㒞㒛㒚㒘㒝㒢㒡㒝㒟㒙㒚㒢㒞㒟㒚㒙㒟㒦㒗㒟㒣㒛㒠㒗㒠㒚㒦㒥㒞㒠㒞㒛㒞㒚㒡㒗㒟㒣㒚㒞㒚㒘㒠㒣㒟㒞㒡㒚㒙㒦㒠㒙㒥㒤㒞㒟㒞㒚㒞㒙㒡㒗㒝㒢㒠㒜㒣㒥㒥㒣㒣㒞㒗㒥㒚㒝㒢㒘㒞㒣㒞㒞㒞㒟㒥㒚㒟㒦㒛㒠㒣㒢㒦㒠㒦㒛㒞㒦㒞㒡㒞㒡㒡㒝㒣㒙㒢㒢㒡㒞㒡㒚㒝㒥㒠㒟㒣㒡㒦㒟㒡㒚㒞㒥㒞㒠㒞㒟㒟㒛㒞㒦㒗㒗㒛㒘㒝㒢㒞㒝㒞㒘㒞㒗㒟㒤㒢㒟㒢㒘㒣㒦㒤㒠㒣㒜㒜㒗㒢㒟㒦㒜㒟㒘㒜㒢㒢㒞㒚㒘㒣㒤㒠㒠㒠㒣㒢㒞㒞㒙㒞㒤㒞㒥㒥㒠㒟㒜㒛㒦㒣㒠㒥㒦㒥㒡㒞㒜㒞㒗㒞㒦㒡㒤㒗㒟㒢㒚㒗㒦㒘㒟㒣㒛㒜㒤㒥㒚㒢㒥㒞㒠㒞㒛㒞㒜㒥㒗㒟㒣㒛㒝㒣㒢㒟㒝㒥㒘㒞㒣㒞㒞㒞㒝㒦㒛㒢㒦㒢㒡㒞㒙㒥㒦㒣㒢㒢㒦㒟㒢㒟㒜㒞㒗㒞㒢㒞㒣㒝㒞㒡㒘㒛㒤㒦㒠㒚㒙㒜㒦㒜㒞㒤㒚㒥㒦㒢㒡㒣㒛㒝㒤㒟㒠㒤㒜㒚㒦㒥㒢㒥㒘㒟㒤㒚㒞㒞㒙㒞㒤㒞㒣㒟㒠㒢㒛㒢㒤㒣㒢㒦㒝㒢㒘㒠㒢㒟㒛㒡㒘㒟㒤㒡㒞㒦㒞㒛㒞㒢㒙㒞㒤㒞㒟㒞㒟㒘㒜㒡㒗㒝㒢㒜㒛㒥㒡㒤㒜㒞㒗㒞㒢㒞㒢㒛㒟㒝㒚㒜㒥㒙㒟㒣㒜㒗㒟㒟㒚㒡㒥㒞㒠㒞㒛㒞㒚㒥㒗㒣㒣㒢㒗㒟㒣㒣㒝㒞㒘㒞㒣㒞㒤㒢㒠㒗㒛㒡㒥㒡㒡㒝㒜㒠㒦㒢㒞㒜㒜㒥㒗㒥㒟㒝㒝㒥㒗㒟㒡㒣㒜㒦㒦㒠㒥㒣㒟㒘㒛㒦㒤㒣㒡㒙㒝㒠㒡㒗㒛㒞㒦㒞㒡㒞㒣㒥㒝㒣㒘㒠㒣㒦㒟㒝㒚㒝㒥㒙㒞㒗㒘㒢㒜㒦㒚㒤㒥㒞㒠㒞㒛㒞㒚㒟㒘㒛㒣㒝㒞㒣㒙㒜㒤㒢㒣㒛㒤㒘㒞㒞㒙㒞㒤㒞㒤㒡㒡㒣㒜㒠㒦㒤㒡㒟㒜㒡㒗㒣㒠㒥㒞㒣㒙㒗㒘㒛㒘㒦㒣㒞㒞㒞㒙㒞㒘㒥㒥㒣㒡㒢㒚㒛㒗㒝㒢㒣㒝㒡㒗㒣㒤㒠㒗㒦㒢㒞㒝㒞㒘㒞㒙㒠㒥㒗㒠㒢㒗㒜㒥㒠㒡㒦㒜㒝㒗㒠㒡㒘㒦㒞㒦㒥㒜㒢㒗㒞㒢㒞㒝㒞㒜㒦㒙㒣㒤㒟㒟㒢㒤㒟㒠㒗㒚㒞㒥㒞㒠㒞㒟㒠㒝㒝㒗㒢㒤㒗㒛㒤㒙㒝㒤㒠㒞㒡㒙㒣㒙㒛㒙㒤㒤㒞㒟㒞㒚㒞㒚㒠㒦㒣㒢㒛㒝㒝㒘㒢㒢㒣㒗㒟㒢㒦㒝㒞㒘㒞㒣㒞㒢㒦㒠㒣㒛㒛㒥㒟㒡㒜㒜㒝㒗㒗㒡㒢㒣㒦㒢㒢㒜㒞㒗㒞㒢㒞㒢㒡㒞㒣㒚㒢㒣㒞㒠㒠㒛㒗㒦㒛㒠㒟㒜㒠㒘㒗㒠㒞㒜㒟㒘㒠㒣㒢㒛㒡㒦㒤㒤㒠㒞㒟㒚㒛㒤㒣㒙㒟㒤㒢㒟㒞㒚㒞㒥㒞㒗㒢㒢㒗㒝㒛㒗㒣㒜㒟㒗㒢㒢㒞㒝㒞㒘㒞㒘㒞㒤㒟㒠㒠㒛㒢㒚㒛㒚㒥㒥㒞㒠㒞㒛㒞㒛㒤㒗㒣㒢㒡㒞㒢㒙㒝㒤㒠㒛㒡㒞㒛㒟㒚㒙㒞㒤㒞㒟㒞㒠㒤㒚㒗㒤㒠㒢㒤㒛㒢㒘㒚㒢㒦㒞㒡㒗㒝㒢㒡㒝㒠㒘㒝㒣㒥㒙㒢㒤㒞㒟㒞㒚㒞㒚㒚㒦㒣㒡㒤㒝㒢㒜㒛㒜㒥㒗㒞㒢㒞㒝㒞㒞㒡㒚㒝㒥㒜㒠㒜㒚㒣㒥㒡㒡㒢㒘㒚㒠㒢㒛㒞㒦㒞㒡㒞㒠㒦㒝㒣㒘㒟㒣㒢㒘㒟㒣㒦㒞㒞㒙㒞㒤㒞㒣㒠㒡㒝㒛㒢㒘㒗㒟㒥㒞㒗㒘㒠㒣㒝㒟㒠㒢㒢㒝㒞㒘㒞㒣㒞㒢㒡㒟㒟㒛㒡㒥㒦㒝㒚㒦㒛㒠㒞㒛㒞㒦㒞㒗㒟㒣㒞㒞㒗㒥㒝㒤㒥㒞㒣㒙㒠㒤㒦㒠㒝㒛㒝㒦㒙㒡㒡㒘㒝㒝㒦㒛㒠㒦㒞㒡㒞㒜㒞㒞㒝㒙㒡㒚㒦㒙㒗㒣㒞㒞㒞㒙㒞㒘㒠㒦㒝㒠㒢㒝㒗㒤㒤㒢㒝㒝㒠㒗㒡㒢㒣㒜㒥㒢㒦㒝㒞㒘㒞㒣㒞㒣㒗㒠㒜㒛㒡㒦㒢㒠㒟㒜㒜㒦㒡㒡㒣㒛㒥㒡㒡㒜㒞㒗㒞㒢㒞㒡㒣㒝㒡㒘㒞㒦㒠㒙㒤㒤㒞㒟㒞㒚㒞㒜㒡㒦㒦㒡㒟㒜㒢㒘㒝㒣㒥㒢㒛㒢㒤㒝㒞㒘㒞㒣㒞㒥㒦㒠㒞㒚㒡㒥㒟㒡㒚㒜㒚㒥㒤㒛㒞㒦㒞㒡㒞㒜㒞㒗㒞㒢㒞㒞㒢㒜㒞㒘㒥㒟㒗㒙㒞㒤㒞㒟㒞㒠㒡㒛㒦㒦㒟㒢㒠㒜㒟㒗㒡㒣㒢㒝㒣㒙㒠㒢㒥㒙㒙㒣㒞㒞㒞㒙㒞㒙㒚㒥㒣㒠㒟㒛㒢㒦㒣㒢㒠㒜㒠㒘㒝㒢㒟㒞㒠㒘㒢㒚㒦㒘㒥㒣㒞㒞㒞㒙㒞㒚㒢㒦㒗㒡㒡㒛㒡㒗㒝㒢㒠㒜㒢㒡㒟㒝㒗㒗㒞㒢㒞㒝㒞㒝㒥㒚㒝㒥㒠㒠㒙㒛㒡㒦㒞㒠㒟㒛㒡㒦㒣㒣㒠㒗㒜㒡㒞㒜㒞㒗㒞㒗㒜㒣㒣㒟㒥㒚㒢㒥㒝㒠㒜㒛㒡㒦㒝㒠㒤㒜㒢㒥㒘㒠㒡㒛㒝㒦㒜㒙㒦㒘㒘㒢㒞㒝㒞㒘㒞㒘㒙㒥㒗㒟㒡㒛㒙㒤㒞㒡㒚㒛㒟㒘㒗㒡㒣㒝㒠㒦㒥㒜㒣㒗㒞㒢㒞㒝㒞㒜㒦㒚㒝㒥㒜㒟㒣㒜㒗㒜㒦㒛㒜㒥㒞㒠㒞㒛㒞㒜㒥㒗㒟㒣㒛㒝㒣㒙㒡㒣㒣㒟㒜㒚㒡㒤㒣㒜㒝㒚㒦㒦㒢㒡㒢㒜㒞㒣㒚㒜㒙㒦㒞㒡㒞㒜㒞㒛㒡㒙㒗㒤㒢㒟㒗㒛㒘㒤㒣㒠㒜㒛㒡㒥㒦㒡㒗㒜㒞㒘㒠㒜㒘㒦㒞㒡㒞㒜㒞㒛㒥㒘㒣㒤㒢㒝㒡㒙㒣㒥㒠㒠㒤㒛㒗㒥㒡㒠㒣㒠㒛㒡㒞㒛㒞㒦㒞㒡㒞㒠㒦㒞㒣㒙㒛㒣㒟㒟㒜㒚㒝㒥㒗㒟㒢㒙㒠㒦㒝㒡㒝㒜㒢㒥㒞㒡㒟㒝㒠㒘㒢㒜㒟㒘㒘㒢㒞㒝㒞㒘㒞㒘㒘㒥㒡㒠㒝㒛㒜㒣㒢㒠㒣㒛㒡㒗㒝㒡㒢㒜㒣㒡㒟㒜㒥㒗㒞㒢㒞㒝㒞㒞㒤㒚㒠㒥㒝㒠㒛㒙㒠㒣㒥㒞㒠㒥㒟㒠㒦㒛㒞㒦㒞㒡㒞㒢㒗㒞㒗㒗㒚㒢㒣㒟㒞㒙㒝㒥㒙㒡㒗㒗㒚㒠㒟㒚㒞㒥㒞㒠㒞㒠㒠㒜㒣㒘㒞㒣㒚㒞㒗㒘㒡㒣㒟㒟㒢㒙㒣㒤㒢㒞㒡㒛㒢㒦㒝㒡㒠㒛㒟㒦㒥㒡㒣㒣㒦㒢㒙㒜㒞㒗㒞㒢㒞㒢㒚㒟㒝㒙㒡㒤㒟㒠㒚㒙㒞㒦㒚㒠㒟㒝㒗㒦㒣㒢㒠㒣㒦㒡㒢㒜㒞㒗㒞㒢㒞㒤㒥㒞㒟㒚㒗㒥㒢㒡㒠㒥㒝㒟㒞㒚㒞㒥㒞㒦㒢㒢㒡㒜㒤㒣㒞㒣㒗㒞㒡㒤㒞㒣㒦㒞㒟㒚㒠㒥㒛㒠㒚㒚㒣㒦㒡㒡㒡㒘㒚㒠㒥㒛㒞㒦㒞㒡㒞㒡㒙㒝㒣㒚㒗㒡㒢㒟㒝㒚㒥㒥㒜㒡㒠㒤㒦㒟㒞㒚㒞㒥㒞㒤㒠㒢㒝㒜㒢㒙㒗㒠㒥㒟㒗㒙㒠㒤㒝㒝㒥㒣㒣㒞㒞㒙㒞㒤㒞㒤㒛㒡㒝㒜㒜㒦㒣㒣㒗㒡㒛㒢㒙㒜㒞㒗㒞㒢㒞㒡㒟㒞㒢㒚㒛㒥㒗㒠㒜㒙㒠㒥㒣㒡㒛㒜㒝㒗㒢㒡㒣㒙㒚㒢㒚㒜㒞㒗㒞㒢㒞㒢㒗㒟㒜㒚㒤㒥㒝㒠㒙㒚㒣㒤㒡㒠㒣㒜㒠㒗㒤㒡㒣㒝㒠㒙㒠㒜㒥㒗㒞㒢㒞㒝㒞㒝㒞㒚㒚㒤㒟㒡㒗㒚㒣㒦㒠㒡㒡㒘㒚㒠㒣㒛㒞㒦㒞㒡㒞㒡㒠㒞㒗㒘㒥㒣㒦㒟㒢㒛㒠㒟㒙㒙㒞㒤㒞㒟㒞㒡㒚㒛㒣㒦㒟㒡㒢㒜㒣㒘㒠㒣㒡㒞㒢㒘㒟㒤㒢㒟㒡㒠㒦㒞㒦㒙㒞㒤㒞㒟㒞㒟㒡㒛㒡㒗㒠㒡㒣㒝㒜㒥㒥㒣㒣㒞㒗㒝㒛㒞㒙㒘㒞㒣㒞㒞㒞㒟㒡㒚㒦㒥㒣㒠㒡㒜㒙㒦㒡㒡㒟㒝㒚㒘㒚㒢㒣㒞㒠㒟㒦㒝㒥㒘㒞㒣㒞㒞㒞㒟㒦㒛㒢㒦㒢㒡㒞㒙㒘㒣㒝㒞㒝㒛㒥㒡㒣㒜㒞㒗㒞㒢㒞㒢㒡㒞㒡㒚㒝㒥㒠㒟㒣㒗㒚㒠㒗㒚㒞㒥㒞㒠㒞㒢㒥㒜㒟㒘㒚㒣㒙㒞㒡㒙㒞㒣㒣㒞㒣㒙㒢㒞㒟㒚㒦㒤㒞㒟㒞㒚㒞㒜㒞㒦㒟㒢㒡㒝㒢㒗㒣㒢㒠㒞㒗㒙㒜㒠㒜㒞㒡㒚㒝㒥㒛㒜㒝㒛㒠㒥㒟㒡㒥㒘㒝㒗㒣㒠㒙㒙㒡㒤㒥㒠㒤㒞㒘㒦㒣㒥㒠㒘㒢㒣㒞㒞㒞㒙㒞㒘㒦㒥㒣㒠㒟㒛㒢㒝㒦㒜㒘㒦㒞㒡㒞㒜㒞㒞㒗㒙㒡㒤㒚㒞㒡㒚㒚㒥㒝㒠㒡㒛㒣㒦㒠㒠㒣㒝㒠㒠㒣㒛㒞㒦㒞㒡㒞㒡㒣㒛㒢㒙㒗㒤㒛㒛㒠㒦㒚㒞㒡㒙㒞㒤㒞㒟㒞㒠㒟㒜㒞㒗㒗㒞㒚㒦㒡㒡㒞㒜㒞㒗㒞㒙㒜㒣㒣㒟㒥㒞㒛㒟㒗㒙㒞㒤㒞㒟㒞㒟㒛㒛㒟㒦㒥㒢㒜㒝㒗㒘㒢㒣㒣㒝㒢㒘㒣㒢㒥㒘㒦㒣㒞㒞㒞㒙㒞㒙㒛㒦㒝㒡㒤㒛㒣㒗㒡㒢㒞㒜㒟㒘㒛㒜㒟㒗㒢㒢㒞㒝㒞㒘㒞㒚㒞㒤㒟㒠㒠㒛㒢㒡㒚㒚㒞㒥㒞㒠㒞㒛㒠㒙㒥㒡㒞㒜㒞㒗㒞㒢㒠㒝㒞㒘㒞㒣㒞㒟㒠㒜㒤㒤㒞㒟㒞㒚㒞㒦㒛㒠㒞㒛㒞㒦㒞㒡㒞㒜㒞㒗㒞㒢㒞㒝㒞㒘㒞㒣㒞㒞㒞㒙㒞㒤㒞㒟㒞㒚㒞㒥㒟㒠㒞㒛㒞㒦㒞㒡㒞㒜㒞㒘㒠㒢㒞㒝㒞㒘㒟㒣㒞㒡㒞㒙㒞㒤㒞㒟㒞㒛㒠㒥㒞㒠㒞㒛㒟㒦㒞㒣㒚㒜㒞㒗㒞㒢㒞㒟㒤㒘㒞㒣㒞㒞㒟㒙㒞㒥㒗㒟㒞㒚㒟㒥㒞㒢㒟㒛㒞㒦㒢㒡㒡㒜㒞㒗㒞㒢㒞㒞㒗㒘㒞㒣㒟㒞㒞㒙㒞㒥㒟㒟㒞㒚㒞㒥㒞㒠㒟㒛㒞㒦㒞㒡㒞㒜㒠㒚㒥㒢㒞㒝㒟㒘㒞㒣㒟㒞㒞㒙㒞㒤㒞㒠㒠㒝㒣㒥㒞㒠㒟㒛㒞㒛㒙㒡㒞㒜㒞㒗㒞㒣㒠㒝㒞㒘㒞㒣㒟㒞㒞㒞㒜㒤㒞㒟㒞㒚㒞㒦㒠㒠㒞㒛㒞㒦㒠㒡㒞㒠㒛㒗㒞㒢㒞㒝㒞㒘㒞㒣㒞㒞㒞㒙㒟㒤㒞㒟㒠㒚㒞㒥㒟㒠㒞㒜㒠㒦㒞㒡㒞㒜㒟㒗㒞㒣㒗㒝㒞㒘㒞㒣㒞㒡㒞㒙㒞㒤㒞㒟㒟㒚㒞㒛㒢㒠㒞㒝㒥㒦㒞㒢㒠㒜㒞㒗㒞㒢㒟㒝㒞㒚㒘㒣㒞㒞㒞㒙㒞㒦㒞㒟㒞㒚㒞㒥㒟㒠㒞㒛㒟㒦㒞㒢㒘㒜㒞㒘㒠㒢㒞㒝㒞㒘㒡㒣㒞㒣㒣㒙㒞㒤㒞㒟㒞㒚㒞㒥㒞㒠㒞㒛㒟㒦㒞㒡㒡㒜㒞㒗㒠㒢㒞㒟㒞㒚㒛㒣㒞㒞㒟㒙㒞㒤㒟㒟㒞㒟㒛㒥㒞㒢㒞㒝㒟㒦㒞㒡㒠㒜㒞㒗㒟㒢㒞㒟㒣㒘㒞㒣㒞㒠㒦㒙㒞㒤㒠㒟㒞㒚㒠㒥㒞㒠㒠㒛㒞㒘㒞㒣㒛㒜㒞㒗㒡㒢㒞㒝㒠㒘㒞㒘㒞㒞㒞㒛㒞㒦㒟㒟㒞㒚㒡㒥㒞㒠㒡㒛㒞㒙㒠㒡㒞㒜㒠㒚㒥㒢㒞㒝㒣㒘㒞㒣㒞㒞㒞㒙㒞㒤㒞㒟㒞㒛㒞㒥㒞㒠㒡㒛㒞㒦㒣㒡㒞㒜㒟㒗㒞㒢㒞㒞㒟㒘㒞㒣㒞㒞㒞㒙㒟㒤㒞㒟㒞㒚㒞㒥㒞㒠㒡㒛㒞㒦㒞㒡㒞㒞㒚㒗㒞㒢㒞㒝㒞㒝㒥㒣㒢㒞㒞㒙㒞㒤㒞㒤㒜㒠㒟㒜㒛㒦㒣㒙㒙㒦㒞㒡㒟㒝㒙㒗㒞㒢㒞㒝㒞㒝㒚㒚㒝㒤㒡㒟㒟㒛㒚㒤㒞㒡㒚㒛㒟㒘㒗㒡㒣㒝㒠㒤㒚㒜㒣㒗㒞㒢㒞㒝㒞㒝㒛㒘㒡㒣㒙㒟㒣㒜㒗㒗㒠㒚㒣㒥㒞㒠㒞㒛㒞㒛㒛㒘㒝㒣㒤㒝㒣㒥㒡㒚㒦㒘㒥㒣㒞㒞㒞㒙㒞㒙㒞㒦㒚㒠㒟㒝㒗㒦㒣㒢㒠㒝㒡㒦㒥㒜㒣㒗㒞㒢㒞㒝㒞㒝㒛㒚㒝㒥㒤㒟㒣㒗㒥㒟㒟㒚㒦㒥㒞㒠㒞㒛㒞㒛㒛㒘㒝㒣㒤㒝㒣㒙㒡㒤㒞㒞㒟㒚㒛㒙㒛㒙㒦㒤㒞㒟㒞㒚㒞㒙㒠㒦㒟㒡㒡㒝㒙㒘㒞㒢㒟㒝㒡㒙㒙㒝㒟㒘㒣㒣㒞㒞㒞㒙㒞㒙㒛㒦㒝㒡㒤㒛㒣㒣㒣㒣㒠㒗㒗㒡㒞㒜㒞㒗㒞㒗㒥㒤㒝㒟㒠㒚㒙㒥㒡㒠㒞㒚㒟㒥㒡㒠㒣㒢㒦㒡㒙㒛㒞㒦㒞㒡㒞㒠㒥㒝㒣㒙㒢㒡㒡㒞㒦㒚㒗㒥㒚㒟㒢㒛㒠㒥㒣㒡㒜㒛㒘㒠㒟㒞㒚㒦㒣㒡㒞㒜㒞㒗㒞㒗㒛㒤㒝㒟㒤㒙㒣㒡㒠㒙㒟㒤㒣㒟㒞㒚㒞㒥㒞㒥㒛㒢㒝㒝㒤㒗㒣㒟㒦㒢㒛㒢㒢㒝㒞㒘㒞㒣㒞㒤㒥㒟㒟㒛㒛㒥㒣㒝㒚㒥㒦㒠㒞㒛㒞㒦㒞㒥㒟㒢㒡㒞㒢㒙㒗㒤㒤㒞㒟㒚㒢㒤㒣㒜㒚㒤㒣㒟㒞㒚㒞㒥㒞㒗㒞㒡㒟㒝㒗㒘㒠㒣㒡㒢㒛㒢㒢㒝㒞㒘㒞㒣㒞㒥㒥㒟㒟㒛㒗㒦㒢㒚㒟㒥㒤㒠㒞㒛㒞㒦㒞㒦㒞㒢㒟㒞㒠㒘㒣㒤㒜㒟㒢㒣㒟㒞㒣㒙㒞㒤㒞㒟㒞㒟㒛㒜㒝㒗㒤㒡㒣㒙㒟㒙㒠㒜㒣㒗㒞㒢㒞㒝㒞㒝㒛㒚㒝㒥㒤㒟㒣㒘㒗㒜㒦㒚㒣㒥㒞㒠㒞㒛㒞㒛㒛㒘㒝㒣㒤㒝㒣㒥㒢㒚㒦㒘㒢㒣㒞㒞㒞㒙㒞㒛㒜㒥㒟㒡㒛㒛㒣㒣㒚㒛㒠㒦㒞㒡㒞㒜㒞㒝㒝㒦㒥㒘㒛㒘㒢㒣㒞㒞㒞㒙㒞㒙㒚㒦㒗㒡㒤㒛㒣㒥㒥㒛㒣㒦㒞㒡㒞㒜㒞㒜㒛㒙㒝㒤㒤㒞㒣㒦㒤㒞㒟㒚㒘㒤㒞㒟㒞㒚㒞㒙㒢㒦㒣㒡㒟㒜㒡㒘㒢㒣㒗㒞㒤㒘㒟㒤㒢㒞㒣㒙㒟㒞㒞㒙㒞㒤㒞㒠㒠㒝㒦㒥㒞㒠㒟㒛㒞㒘㒗㒡㒞㒜㒞㒗㒞㒤㒞㒟㒛㒘㒞㒣㒟㒞㒞㒙㒟㒤㒞㒟㒦㒚㒞㒥㒤㒥㒙㒛㒞㒦㒟㒡㒞㒝㒘㒗㒞㒢㒟㒝㒞㒘㒞㒣㒞㒞㒢㒙㒡㒤㒞㒟㒞㒚㒞㒦㒘㒠㒞㒛㒟㒦㒞㒢㒠㒟㒦㒗㒞㒢㒟㒝㒞㒘㒢㒣㒞㒞㒞㒙㒞㒤㒤㒠㒚㒚㒞㒥㒞㒠㒞㒜㒘㒦㒞㒡㒟㒜㒞㒗㒟㒢㒞㒝㒢㒘㒡㒣㒞㒞㒞㒙㒞㒥㒘㒟㒞㒚㒟㒥㒞㒡㒠㒞㒦㒦㒞㒡㒟㒜㒞㒙㒗㒢㒞㒝㒞㒘㒞㒦㒞㒡㒠㒙㒞㒤㒟㒟㒞㒚㒦㒥㒞㒠㒠㒛㒞㒦㒢㒡㒡㒜㒞㒗㒞㒢㒞㒣㒞㒘㒞㒣㒟㒞㒞㒚㒠㒗㒦㒟㒞㒚㒟㒥㒞㒢㒗㒛㒞㒦㒞㒡㒞㒞㒞㒙㒛㒢㒞㒝㒟㒘㒞㒣㒟㒞㒞㒙㒦㒤㒞㒡㒤㒝㒜㒥㒞㒠㒟㒛㒞㒗㒝㒡㒞㒜㒟㒗㒞㒢㒠㒝㒞㒘㒢㒣㒡㒞㒞㒙㒞㒤㒞㒠㒝㒚㒞㒥㒟㒠㒞㒛㒢㒦㒡㒡㒞㒜㒞㒗㒞㒘㒞㒝㒞㒘㒟㒣㒞㒟㒠㒜㒦㒤㒞㒟㒟㒚㒞㒥㒢㒠㒞㒛㒞㒦㒞㒡㒤㒝㒚㒗㒞㒢㒞㒝㒞㒞㒞㒣㒞㒞㒟㒙㒞㒤㒟㒟㒞㒚㒢㒥㒡㒠㒞㒛㒞㒦㒞㒗㒞㒜㒞㒗㒟㒢㒞㒞㒠㒛㒦㒣㒞㒞㒟㒙㒞㒦㒗㒟㒞㒚㒞㒥㒞㒣㒞㒞㒠㒦㒞㒡㒟㒜㒞㒗㒦㒢㒞㒞㒛㒘㒞㒤㒠㒡㒦㒙㒞㒤㒟㒟㒞㒜㒗㒥㒞㒠㒞㒛㒞㒘㒞㒣㒛㒜㒞㒗㒟㒢㒞㒝㒟㒘㒞㒣㒦㒞㒞㒙㒤㒙㒙㒟㒞㒚㒟㒥㒞㒦㒞㒛㒞㒦㒟㒡㒞㒜㒞㒗㒞㒢㒢㒝㒡㒘㒞㒣㒞㒞㒞㒟㒞㒤㒞㒟㒟㒚㒞㒦㒠㒣㒦㒛㒞㒦㒟㒡㒞㒝㒠㒗㒞㒢㒞㒝㒞㒙㒠㒥㒤㒞㒞㒙㒠㒤㒞㒠㒞㒚㒞㒥㒞㒠㒞㒝㒞㒦㒞㒡㒞㒜㒠㒗㒞㒢㒠㒝㒞㒘㒤㒣㒞㒠㒞㒙㒞㒤㒞㒟㒠㒚㒞㒥㒠㒠㒞㒛㒡㒦㒞㒣㒞㒜㒞㒗㒞㒢㒠㒝㒞㒘㒠㒣㒞㒟㒗㒙㒞㒦㒞㒟㒞㒚㒞㒥㒠㒠㒞㒛㒠㒦㒞㒢㒚㒜㒞㒗㒞㒢㒞㒝㒞㒘㒠㒣㒞㒞㒡㒙㒞㒤㒞㒟㒞㒚㒞㒥㒞㒠㒞㒛㒟㒦㒞㒡㒞㒜㒞㒗㒡㒢㒞㒝㒢㒘㒞㒣㒞㒞㒞㒙㒞㒚㒛㒟㒞㒚㒟㒥㒞㒢㒞㒝㒛㒦㒞㒡㒤㒜㒞㒗㒣㒢㒞㒝㒟㒘㒞㒤㒠㒡㒦㒙㒞㒤㒥㒟㒞㒛㒣㒥㒞㒠㒞㒛㒞㒦㒤㒣㒝㒜㒞㒗㒤㒢㒞㒢㒗㒘㒞㒣㒟㒞㒞㒙㒥㒤㒞㒟㒢㒚㒡㒥㒞㒠㒞㒛㒞㒛㒗㒡㒞㒜㒟㒗㒞㒤㒞㒟㒛㒘㒞㒣㒤㒞㒞㒙㒣㒤㒞㒟㒟㒚㒞㒦㒠㒣㒦㒛㒞㒦㒥㒡㒞㒝㒜㒗㒞㒢㒞㒝㒞㒘㒤㒥㒝㒞㒞㒙㒤㒤㒞㒤㒗㒚㒞㒥㒟㒠㒞㒛㒥㒦㒞㒡㒢㒜㒡㒗㒞㒢㒞㒝㒞㒝㒗㒣㒞㒞㒟㒙㒞㒦㒞㒡㒛㒚㒞㒥㒤㒠㒞㒛㒣㒦㒞㒡㒟㒜㒞㒘㒠㒥㒦㒝㒞㒘㒥㒣㒞㒞㒣㒙㒞㒤㒞㒟㒞㒚㒤㒦㒚㒠㒞㒛㒤㒦㒞㒤㒜㒜㒞㒗㒟㒢㒞㒝㒥㒘㒞㒣㒢㒞㒡㒙㒞㒤㒞㒟㒞㒝㒜㒥㒞㒠㒟㒛㒞㒦㒢㒡㒡㒜㒞㒗㒞㒢㒞㒢㒗㒘㒞㒣㒟㒞㒞㒛㒞㒦㒛㒟㒞㒚㒤㒥㒞㒠㒣㒛㒞㒦㒟㒡㒞㒝㒠㒚㒦㒢㒞㒝㒥㒘㒞㒤㒥㒞㒞㒙㒞㒤㒞㒟㒤㒜㒝㒥㒞㒠㒤㒛㒞㒛㒗㒡㒞㒜㒟㒗㒞㒢㒥㒝㒞㒘㒢㒣㒡㒞㒞㒙㒞㒤㒞㒤㒗㒚㒞㒥㒟㒠㒞㒝㒞㒘㒛㒡㒞㒜㒤㒗㒞㒢㒣㒝㒞㒘㒟㒣㒞㒟㒠㒜㒦㒤㒞㒟㒥㒚㒞㒦㒘㒠㒞㒛㒞㒦㒞㒡㒤㒝㒚㒗㒞㒢㒤㒝㒞㒛㒥㒣㒞㒞㒟㒙㒞㒤㒥㒟㒞㒚㒢㒥㒡㒠㒞㒛㒞㒦㒞㒤㒥㒜㒞㒗㒟㒢㒞㒝㒢㒘㒡㒣㒞㒞㒞㒙㒞㒙㒗㒟㒞㒚㒟㒥㒞㒢㒞㒝㒛㒦㒞㒡㒤㒜㒞㒗㒣㒢㒞㒝㒟㒘㒞㒤㒠㒡㒦㒙㒞㒤㒥㒟㒞㒜㒙㒥㒞㒠㒞㒛㒞㒦㒤㒣㒝㒜㒞㒗㒤㒢㒞㒢㒗㒘㒞㒣㒟㒞㒞㒙㒥㒤㒞㒟㒢㒚㒡㒥㒞㒠㒞㒛㒞㒛㒗㒡㒞㒜㒟㒗㒞㒤㒞㒟㒛㒘㒞㒣㒤㒞㒞㒙㒣㒤㒞㒟㒟㒚㒞㒦㒠㒣㒦㒛㒞㒦㒥㒡㒞㒜㒥㒗㒞㒢㒞㒝㒞㒘㒤㒤㒚㒞㒞㒙㒤㒤㒞㒣㒞㒚㒞㒥㒟㒠㒞㒛㒥㒦㒞㒡㒢㒜㒡㒗㒞㒢㒞㒝㒞㒜㒞㒣㒞㒞㒟㒙㒞㒤㒢㒟㒡㒚㒞㒥㒞㒠㒞㒠㒗㒦㒞㒡㒟㒜㒞㒙㒞㒤㒛㒝㒞㒘㒤㒣㒞㒞㒣㒙㒞㒤㒟㒟㒞㒛㒠㒘㒦㒠㒞㒛㒥㒦㒞㒢㒝㒜㒞㒗㒞㒢㒞㒝㒤㒚㒝㒣㒞㒞㒤㒙㒞㒙㒗㒟㒞㒚㒟㒥㒞㒠㒥㒛㒞㒦㒢㒡㒡㒜㒞㒗㒞㒢㒞㒢㒗㒘㒞㒣㒟㒞㒞㒛㒞㒦㒛㒟㒞㒚㒤㒥㒞㒠㒣㒛㒞㒦㒟㒡㒞㒝㒠㒚㒦㒢㒞㒝㒥㒘㒞㒤㒤㒞㒞㒙㒞㒤㒞㒟㒤㒜㒝㒥㒞㒠㒤㒛㒞㒛㒗㒡㒞㒜㒟㒗㒞㒢㒥㒝㒞㒘㒢㒣㒡㒞㒞㒙㒞㒤㒞㒤㒗㒚㒞㒥㒟㒠㒞㒛㒢㒦㒡㒡㒞㒜㒞㒗㒞㒘㒛㒝㒞㒘㒟㒣㒞㒟㒠㒜㒦㒤㒞㒟㒤㒚㒞㒦㒞㒠㒞㒛㒞㒦㒞㒣㒞㒟㒘㒗㒞㒢㒤㒝㒞㒘㒤㒣㒞㒟㒙㒙㒞㒦㒞㒟㒞㒚㒞㒥㒤㒠㒞㒛㒤㒦㒞㒣㒘㒜㒞㒘㒠㒢㒞㒝㒞㒘㒥㒣㒞㒟㒞㒙㒞㒤㒞㒟㒞㒜㒞㒥㒞㒠㒞㒛㒥㒦㒞㒡㒥㒜㒞㒗㒤㒢㒞㒟㒞㒘㒞㒣㒞㒞㒥㒙㒞㒤㒥㒟㒞㒚㒡㒥㒞㒢㒞㒛㒞㒦㒞㒡㒥㒜㒞㒗㒥㒢㒞㒞㒦㒘㒞㒣㒞㒞㒞㒙㒞㒤㒤㒟㒞㒚㒤㒥㒞㒠㒥㒛㒞㒗㒞㒡㒞㒜㒞㒗㒣㒢㒞㒞㒢㒘㒞㒣㒤㒞㒞㒛㒞㒤㒞㒟㒞㒚㒤㒥㒞㒠㒣㒛㒞㒗㒟㒡㒞㒜㒞㒗㒞㒢㒞㒝㒤㒘㒞㒣㒠㒞㒞㒙㒟㒤㒞㒡㒞㒚㒞㒥㒞㒠㒤㒛㒞㒦㒣㒡㒞㒞㒚㒗㒞㒢㒞㒝㒞㒘㒞㒣㒤㒞㒞㒙㒠㒤㒞㒟㒟㒚㒞㒦㒠㒠㒞㒛㒞㒦㒤㒡㒞㒝㒡㒗㒞㒢㒞㒝㒞㒘㒞㒣㒞㒞㒞㒙㒤㒤㒞㒟㒟㒚㒞㒥㒟㒠㒞㒜㒠㒦㒞㒡㒞㒜㒤㒗㒞㒣㒞㒝㒞㒘㒞㒣㒞㒠㒞㒙㒞㒤㒞㒟㒤㒚㒞㒥㒤㒠㒞㒛㒤㒦㒞㒣㒞㒜㒞㒗㒞㒢㒤㒝㒞㒘㒤㒣㒞㒞㒡㒙㒞㒦㒞㒟㒞㒚㒞㒥㒤㒠㒞㒛㒤㒦㒞㒢㒗㒜㒞㒘㒞㒢㒞㒝㒞㒘㒣㒣㒞㒟㒢㒙㒞㒤㒤㒟㒞㒚㒤㒚㒗㒠㒞㒛㒟㒦㒞㒣㒟㒜㒞㒗㒟㒢㒞㒝㒠㒘㒞㒣㒢㒞㒡㒙㒞㒤㒞㒟㒞㒜㒟㒥㒞㒠㒟㒛㒞㒦㒢㒡㒡㒜㒞㒗㒞㒢㒞㒞㒢㒘㒞㒣㒟㒞㒞㒙㒞㒥㒟㒟㒞㒚㒞㒥㒞㒠㒟㒛㒞㒦㒞㒡㒞㒜㒟㒗㒞㒢㒞㒝㒞㒘㒞㒣㒦㒞㒞㒙㒞㒤㒞㒤㒤㒚㒞㒥㒞㒠㒞㒛㒞㒦㒞㒡㒞㒛㒞㒛㒝㒟㒥㒝㒞㒘㒞㒣㒞㒞㒞㒙㒞㒤㒞㒦㒞㒞㒞㒝㒠㒠㒢㒛㒞㒦㒞㒡㒞㒢㒠㒟㒗㒙㒢㒣㒣㒘㒟㒣㒞㒞㒞㒙㒞㒤㒞㒟㒟㒚㒤㒥㒞㒠㒞㒛㒞㒝㒡㒘㒢㒣㒠㒞㒗㒙㒜㒣㒥㒘㒟㒣㒡㒞㒞㒙㒞㒤㒞㒦㒡㒡㒣㒛㒠㒣㒚㒜㒚㒦㒞㒡㒞㒜㒞㒝㒤㒗㒗㒡㒠㒟㒤㒘㒢㒥㒚㒟㒦㒛㒡㒤㒝㒟㒡㒚㒠㒥㒝㒠㒥㒦㒢㒡㒞㒜㒞㒗㒞㒘㒡㒣㒦㒞㒟㒚㒠㒠㒠㒙㒞㒤㒞㒟㒞㒛㒠㒘㒦㒠㒞㒛㒡㒦㒞㒡㒥㒜㒞㒗㒞㒢㒞㒝㒞㒙㒠㒣㒞㒞㒡㒙㒞㒤㒡㒟㒞㒚㒟㒥㒞㒠㒤㒛㒥㒦㒞㒡㒡㒜㒞㒗㒣㒢㒞㒝㒟㒘㒞㒣㒟㒞㒞㒙㒢㒤㒡㒟㒞㒚㒞㒥㒞㒠㒣㒛㒞㒦㒟㒡㒞㒜㒢㒗㒡㒢㒞㒝㒞㒘㒞㒣㒦㒞㒞㒙㒟㒤㒞㒠㒠㒝㒦㒥㒞㒠㒡㒛㒞㒦㒥㒡㒞㒜㒞㒗㒞㒢㒞㒞㒠㒘㒞㒣㒡㒞㒞㒙㒡㒤㒞㒟㒟㒚㒞㒥㒞㒥㒣㒛㒞㒦㒡㒡㒞㒜㒠㒗㒞㒢㒞㒝㒞㒙㒠㒗㒞㒞㒞㒙㒡㒤㒞㒟㒟㒚㒞㒥㒞㒠㒞㒜㒠㒚㒜㒡㒞㒜㒢㒗㒞㒢㒢㒝㒞㒘㒞㒣㒞㒟㒠㒙㒞㒤㒞㒟㒣㒚㒞㒥㒟㒠㒞㒛㒞㒦㒞㒡㒞㒜㒞㒗㒞㒢㒤㒝㒞㒘㒞㒣㒞㒞㒞㒙㒞㒥㒠㒟㒞㒚㒞㒥㒥㒠㒞㒛㒟㒦㒞㒡㒞㒜㒞㒗㒢㒢㒞㒝㒞㒘㒣㒣㒞㒠㒜㒙㒞㒤㒟㒟㒞㒚㒞㒦㒢㒠㒞㒜㒗㒦㒞㒡㒢㒜㒞㒗㒞㒢㒞㒞㒠㒚㒚㒣㒞㒟㒘㒙㒞㒤㒣㒟㒞㒚㒞㒥㒞㒢㒞㒛㒞㒦㒞㒢㒘㒜㒞㒘㒘㒢㒞㒝㒦㒘㒞㒥㒞㒞㒞㒙㒞㒥㒙㒟㒞㒚㒞㒥㒞㒠㒤㒛㒞㒦㒞㒡㒞㒜㒞㒘㒛㒢㒞㒝㒦㒘㒞㒣㒞㒞㒞㒙㒞㒤㒞㒟㒞㒛㒜㒥㒞㒠㒦㒛㒞㒦㒞㒡㒞㒜㒞㒗㒞㒢㒞㒞㒙㒘㒞㒤㒜㒞㒞㒙㒠㒤㒞㒡㒞㒚㒞㒥㒞㒡㒙㒛㒞㒗㒙㒡㒞㒜㒡㒗㒞㒢㒞㒝㒞㒘㒞㒤㒙㒞㒞㒙㒠㒤㒞㒟㒠㒚㒞㒥㒞㒠㒞㒛㒞㒗㒙㒡㒞㒝㒙㒗㒞㒢㒡㒝㒞㒚㒞㒣㒞㒞㒞㒚㒙㒤㒞㒠㒙㒚㒞㒥㒠㒠㒞㒛㒞㒦㒞㒡㒞㒝㒘㒗㒞㒢㒠㒝㒞㒘㒠㒣㒞㒞㒞㒙㒞㒤㒞㒟㒢㒚㒞㒦㒗㒠㒞㒜㒘㒦㒞㒡㒞㒜㒞㒗㒞㒣㒗㒝㒞㒘㒡㒣㒞㒞㒠㒙㒞㒦㒞㒟㒞㒚㒞㒥㒡㒠㒞㒜㒗㒦㒞㒡㒠㒜㒞㒗㒢㒤㒜㒝㒞㒘㒣㒣㒞㒟㒜㒙㒞㒤㒟㒟㒞㒛㒠㒘㒦㒠㒞㒛㒣㒦㒞㒡㒥㒜㒞㒗㒞㒢㒞㒝㒞㒜㒡㒣㒞㒞㒣㒙㒞㒤㒟㒟㒞㒚㒢㒥㒞㒠㒞㒠㒣㒦㒞㒡㒢㒜㒞㒗㒠㒢㒞㒝㒞㒘㒞㒣㒞㒟㒟㒙㒞㒤㒞㒟㒞㒚㒟㒥㒞㒠㒞㒛㒞㒦㒡㒡㒞㒜㒞㒗㒞㒢㒞㒝㒠㒘㒞㒣㒞㒞㒞㒤㒛㒤㒣㒟㒞㒚㒞㒥㒞㒗㒞㒡㒡㒜㒟㒘㒚㒣㒚㒗㒞㒢㒞㒝㒞㒘㒞㒣㒞㒞㒞㒙㒞㒤㒞㒟㒞㒜㒜㒥㒞㒠㒞㒛㒞㒗㒠㒥㒞㒜㒞㒗㒠㒢㒞㒝㒠㒘㒞㒣㒞㒞㒞㒚㒠㒘㒞㒟㒞㒚㒡㒥㒞㒠㒠㒛㒞㒦㒞㒡㒞㒝㒠㒚㒦㒢㒞㒝㒢㒘㒞㒣㒟㒞㒞㒙㒞㒤㒞㒟㒤㒞㒠㒥㒞㒠㒣㒛㒞㒦㒞㒡㒞㒜㒟㒗㒞㒢㒢㒝㒞㒘㒞㒦㒚㒞㒞㒙㒞㒤㒞㒟㒠㒚㒞㒥㒞㒠㒞㒛㒞㒙㒚㒡㒞㒜㒞㒗㒞㒢㒞㒝㒞㒘㒞㒣㒞㒞㒞㒜㒚㒤㒞㒟㒞㒚㒞㒥㒡㒠㒞㒛㒞㒦㒞㒡㒞㒟㒚㒗㒞㒢㒞㒝㒞㒘㒟㒣㒞㒞㒞㒙㒞㒤㒞㒤㒝㒚㒞㒥㒢㒠㒞㒛㒠㒦㒞㒡㒟㒜㒞㒗㒤㒤㒝㒝㒞㒘㒞㒣㒞㒟㒚㒙㒞㒤㒟㒟㒞㒚㒟㒥㒞㒠㒢㒛㒡㒦㒞㒡㒞㒜㒞㒘㒚㒢㒞㒝㒟㒘㒞㒣㒢㒞㒡㒙㒞㒤㒞㒟㒞㒜㒘㒥㒞㒠㒟㒛㒞㒦㒤㒣㒝㒜㒞㒗㒞㒢㒞㒞㒝㒘㒞㒣㒟㒞㒞㒙㒟㒤㒞㒟㒢㒚㒡㒥㒞㒠㒞㒛㒞㒗㒝㒡㒞㒜㒟㒗㒞㒢㒢㒝㒡㒘㒞㒣㒞㒞㒞㒛㒘㒤㒞㒟㒟㒚㒞㒥㒤㒢㒝㒛㒞㒦㒟㒡㒞㒝㒠㒗㒞㒢㒟㒝㒞㒘㒞㒣㒞㒞㒢㒙㒡㒤㒞㒟㒞㒚㒞㒦㒠㒠㒞㒛㒟㒦㒞㒡㒢㒜㒡㒗㒞㒢㒞㒝㒞㒚㒘㒣㒞㒞㒟㒙㒞㒤㒞㒤㒟㒚㒞㒥㒢㒠㒞㒛㒠㒦㒞㒡㒡㒜㒞㒗㒞㒗㒟㒝㒞㒘㒣㒣㒞㒞㒡㒙㒞㒤㒠㒟㒞㒚㒤㒦㒚㒠㒞㒛㒢㒦㒞㒣㒘㒜㒞㒗㒟㒢㒞㒝㒣㒘㒞㒣㒢㒞㒡㒙㒞㒤㒞㒟㒞㒜㒘㒥㒞㒠㒟㒛㒞㒦㒞㒦㒟㒜㒞㒗㒢㒢㒞㒝㒠㒘㒞㒣㒡㒞㒞㒙㒞㒙㒟㒟㒞㒚㒣㒥㒞㒠㒡㒛㒞㒦㒠㒡㒞㒜㒤㒙㒝㒢㒞㒝㒢㒘㒞㒥㒙㒞㒞㒙㒟㒤㒞㒟㒣㒚㒞㒥㒢㒠㒡㒛㒞㒦㒞㒡㒞㒞㒙㒗㒞㒢㒟㒝㒞㒘㒞㒘㒢㒞㒞㒙㒢㒤㒞㒟㒞㒚㒞㒥㒞㒠㒞㒛㒞㒙㒗㒡㒞㒜㒢㒗㒞㒢㒟㒝㒞㒘㒞㒣㒞㒞㒞㒞㒣㒤㒞㒟㒢㒚㒞㒥㒠㒠㒞㒛㒞㒦㒞㒡㒞㒝㒟㒗㒞㒢㒞㒝㒞㒘㒟㒣㒞㒞㒞㒙㒞㒤㒠㒟㒟㒚㒞㒥㒞㒠㒞㒛㒞㒦㒞㒡㒞㒜㒞㒗㒥㒢㒞㒝㒞㒘㒞㒣㒞㒞㒤㒙㒞㒤㒞㒟㒞㒚㒟㒥㒞㒠㒞㒛㒞㒦㒞㒡㒞㒜㒞㒗㒞㒢㒞㒝㒞㒘㒞㒣㒞㒞㒞㒙㒞㒤㒞㒟㒞㒚㒞㒥㒞㒠㒞㒛㒞㒦㒞㒡㒞㒜㒞㒗㒞㒢㒞㒝㒞㒘㒞㒣㒡㒞㒞㒙㒞㒤㒞㒟㒞㒚㒞㒥㒞㒠㒞㒛㒞㒦㒞㒡㒞㒜㒞㒗㒞㒢㒞㒝㒞㒘㒞㒣㒞㒞㒞㒙㒠㒤㒞㒟㒞㒚㒞㒥㒞㒠㒞㒛㒞㒦㒞㒡㒞㒜㒟㒗㒞㒢㒞㒝㒞㒘㒞㒣㒞㒞㒞㒙㒞㒤㒞");local _l_ll=(0xdf-(146+-#{(function()return{','}end)(),76;{}}))local _ll=105 local __=__l;local _={}_={[((6080/0x98)+-#"I have 0x in my nickname and I am cool.")]=function()local _lll,__l,_l,_=___lll(__l_ll,__,__+__l__);__=__+_ll__;_ll=(_ll+(_l_ll*_ll__))%_l_;return(((_+_ll-(_l_ll)+___*(_ll__*__ll))%___)*((__ll*_ll_ll)^__ll))+(((_l+_ll-(_l_ll*__ll)+___*(__ll^__l__))%_l_)*(___*_l_))+(((__l+_ll-(_l_ll*__l__)+_ll_ll)%_l_)*___)+((_lll+_ll-(_l_ll*_ll__)+_ll_ll)%_l_);end,[(-#"<@!761654159095103499> send toe nail pics"+(0x95-106))]=function(_,_,_)local _=___lll(__l_ll,__,__);__=__+_lll;_ll=(_ll+(_l_ll))%_l_;return((_+_ll-(_l_ll)+_ll_ll)%___);end,[(0x24+-33)]=function()local _l,_=___lll(__l_ll,__,__+__ll);_ll=(_ll+(_l_ll*__ll))%_l_;__=__+__ll;return(((_+_ll-(_l_ll)+___*(__ll*_ll__))%___)*_l_)+((_l+_ll-(_l_ll*__ll)+_l_*(__ll^__l__))%___);end,[(0x51-77)]=function(__,_,_l)if _l then local _=(__/__ll^(_-__l))%__ll^((_l-_lll)-(_-__l)+_lll);return _-_%__l;else local _=__ll^(_-_lll);return(__%(_+_)>=_)and __l or _____;end;end,[((0x8a0/48)+-#[[MoonSec V3 cracked download not clickbait]])]=function()local _l=_[(0x4d/77)]();local __=_[(-0x57+88)]();local _l_l=__l;local _ll=(_[(0x21-29)](__,_lll,_l_lll+_ll__)*(__ll^(_l_lll*__ll)))+_l;local _l=_[(-0x55+89)](__,21,31);local _=((-__l)^_[(-106+0x6e)](__,32));if(_l==_____)then if(_ll==_lllll)then return _*_____;else _l=_lll;_l_l=_lllll;end;elseif(_l==(___*(__ll^__l__))-_lll)then return(_ll==_____)and(_*(_lll/_lllll))or(_*(_____/_lllll));end;return _ll__l(_,_l-((_l_*(_ll__))-__l))*(_l_l+(_ll/(__ll^___l_l)));end,[(0x108/44)]=function(_l,__ll,__ll)local __ll;if(not _l)then _l=_[(0x2b/43)]();if(_l==_____)then return'';end;end;__ll=_l_l_l(__l_ll,__,__+_l-__l);__=__+_l;local _=''for _l=_lll,#__ll do _=__ll_l(_,_l__ll((___lll(_l_l_l(__ll,_l,_l))+_ll)%_l_))_ll=(_ll+_l_ll)%___ end return _;end}local function __l_ll(...)return{...},____ll('#',...)end local function _ll_ll()local _llll={};local __l_={};local _l={};local __lll={_llll,__l_,nil,_l};local __={}local _l_ll=(0x73-92)local _ll={[(872/((-112+0x17a)+-#[[Fun and games until a = (function() a() end) a()]]))]=(function(_l)return not(#_l==_[((128-0x62)+-#[[FEDERAL IS A FUCKING SCAMMER]])]())end),[(-0x77+119)]=(function(_l)return _[(0x28+-35)]()end),[(-#"staymad"+(0x38-48))]=(function(_l)return _[(126/0x15)]()end),[(-#"i love perth"+(0xa8/12))]=(function(_l)local __=_[(34-0x1c)]()local _=''local _l=1 for _ll=1,#__ do _l=(_l+_l_ll)%_l_ _=__ll_l(_,_l__ll((___lll(__:sub(_ll,_ll))+_l)%___))end return _ end)};local _l=_[(42-0x29)]()for _l=1,_l do local _=_[(-#[[This file has been enchanted with uncrackable V, fuck the fuck off]]+(-84+0x98))]();local __l;local _=_ll[_%(387/0x9)];__[_l]=_ and _({});end;for __l_=1,_[(97/0x61)]()do local _l=_[(113-0x6f)]();if(_[(-90+0x5e)](_l,__l,_lll)==_lllll)then local _l_=_[(34-0x1e)](_l,__ll,__l__);local _ll=_[(1012/0xfd)](_l,_ll__,__ll+_ll__);local _l={_[(0x195/((33124/0xa9)+-#'psu got dumped so hard their entire source code came out rofl'))](),_[(-#"Pain is an illusion created by your brain"+(0xfd0/92))](),nil,nil};local ___={[(0x5a+-90)]=function()_l[__l_l]=_[(-#'fortnite balls'+(0x693/99))]();_l[_lll_]=_[(-#[[<@!519139355118534656> stop with the cap ms v3 got my script 30.0 ms]]+(0xb5f/41))]();end,[((0xb1-137)+-#'i know what sex is, but i wont tell you')]=function()_l[_l_l]=_[(-#'Shouldve invite FBI Bot'+(117-0x5d))]();end,[((0x70c/41)+-#[[pssssst the wrapper function is over there]])]=function()_l[_l_l]=_[(0xc8/200)]()-(__ll^_l_lll)end,[(27-0x18)]=function()_l[____]=_[(98/0x62)]()-(__ll^_l_lll)_l[_l___]=_[(0x27-36)]();end};___[_l_]();if(_[((0x3f+-16)+-#[[Imagine being named omer faruk birer aka RY]])](_ll,_lll,__l)==_lll)then _l[_ll_]=__[_l[___l]]end if(_[((0x63+-82)+-#"bit.bdiv(0,0)")](_ll,__ll,__ll)==__l)then _l[_ll_l]=__[_l[_l__]]end if(_[(0x48+(-17000/0xfa))](_ll,__l__,__l__)==_lll)then _l[__ll_]=__[_l[_lll_]]end _llll[__l_]=_l;end end;__lll[3]=_[((-0x2b+57)+-#[[mom shot dad]])]();for _=_lll,_[((10478/0xa9)+-#[[psu got dumped so hard their entire source code came out rofl]])]()do __l_[_-_lll]=_ll_ll();end;return __lll;end;local function _____(_,_ll__,_l_ll)local __=_[__ll];local _l_=_[__l__];local _=_[__l];return(function(...)local _l__ll={};local ___=_;local ___lll=__l_ll local _ll=__l;local _lllll=__;local __={};local _=__l _*=-1 local __l__=_;local _l_lll={};local __l_ll=____ll('#',...)-_lll;local _ll_ll={...};local _l_=_l_;for _=0,__l_ll do if(_>=_l_)then _l__ll[_-_l_]=_ll_ll[_+_lll];else __[_]=_ll_ll[_+__l];end;end;local _=__l_ll-_l_+__l local _;local _l_;while true do _=___[_ll];_l_=_[(68-0x43)];_l=(992180)while _l_<=(-#[[can someone send me the psu source code it got deletedd]]+(0xfc-155))do _l-= _l _l=(3898335)while(0xff0/204)>=_l_ do _l-= _l _l=(438620)while(2268/0xfc)>=_l_ do _l-= _l _l=(2271250)while(-#'perth thinks psu is bad (it is) and uses ms priv'+(-60+0x70))>=_l_ do _l-= _l _l=(3674405)while(0xaa/170)>=_l_ do _l-= _l _l=(1318618)while _l_>(0x0/151)do _l-= _l __[_[_ll_]]=__[_[____]][_[____l]];break end while 1942==(_l)/((0x581-730))do __[_[___l]]=#__[_[_llll]];break end;break;end while(_l)/((254009/0x83))==1895 do _l=(8867236)while(-#[[i loooove federal]]+(70-(0x8a+-87)))>=_l_ do _l-= _l if(__[_[_l__l]]~=_[____l])then _ll=_ll+_lll;else _ll=_[_llll];end;break;end while 3934==(_l)/((0x93e+-112))do _l=(2578842)while _l_>(0x65-98)do _l-= _l local _=_[___ll]__[_]=__[_](__[_+_lll])break end while(_l)/((-0x15+1920))==1358 do _ll=_[_l__];break end;break;end break;end break;end while(_l)/((0x8fe3f/205))==790 do _l=(8721807)while _l_<=((0x6c-78)+-#"Why are you reading this")do _l-= _l _l=(2176200)while _l_>(-#'how many meme strings do we have'+(-101+0x8a))do _l-= _l __[_[__lll]]=_ll__[_[_l__]];_ll=_ll+__l;_=___[_ll];__[_[_ll_]]=#__[_[_l_l]];_ll=_ll+__l;_=___[_ll];_ll__[_[_l_l]]=__[_[___l]];_ll=_ll+__l;_=___[_ll];__[_[___l]]=_ll__[_[__l_l]];_ll=_ll+__l;_=___[_ll];__[_[__l_]]=#__[_[____]];_ll=_ll+__l;_=___[_ll];_ll__[_[_l__]]=__[_[__lll]];_ll=_ll+__l;_=___[_ll];do return end;break end while(_l)/((3417+-0x45))==650 do __[_[___l]]=__[_[_llll]][__[_[_l_l_]]];break end;break;end while(_l)/((-#"no i legit burned it"+(0x64290/144)))==3083 do _l=(29016)while _l_<=(0x540/192)do _l-= _l if not __[_[___l]]then _ll=_ll+_lll;else _ll=_[_l__];end;break;end while 52==(_l)/((1202-0x284))do _l=(1743360)while _l_>(0x53+-75)do _l-= _l __[_[_ll_]][_[_l__]]=_[____l];break end while 960==(_l)/((0xe67-1871))do __[_[__lll]]=(_[_l_l]~=0);_ll=_ll+_lll;break end;break;end break;end break;end break;end while(_l)/((0x3e3+-31))==455 do _l=(3098216)while(2282/0xa3)>=_l_ do _l-= _l _l=(1850144)while _l_<=(-#[[We all Love Child Porn]]+(-0x6e+143))do _l-= _l _l=(1222452)while _l_>(-#[[helloretard will face off against MoonSec if Federal keeps deleting my strings fuck you]]+(4753/0x31))do _l-= _l local _l_=_[__lll];local ___=_[__ll_];local _l=_l_+2 local _l_={__[_l_](__[_l_+1],__[_l])};for _=1,___ do __[_l+_]=_l_[_];end;local _l_=_l_[1]if _l_ then __[_l]=_l_ _ll=_[_l_l];else _ll=_ll+__l;end;break end while(_l)/((0x1bfc-3600))==343 do _ll__[_[_llll]]=__[_[_ll_]];break end;break;end while(_l)/((537472/(0x214-324)))==716 do _l=(5123760)while(888/0x4a)>=_l_ do _l-= _l if(__[_[_ll_]]==__[_[____l]])then _ll=_ll+_lll;else _ll=_[_llll];end;break;end while 2960==(_l)/((0x208a7/77))do _l=(11003499)while(3172/(583-0x153))<_l_ do _l-= _l __[_[__lll]]=_[_llll];break end while(_l)/((-#'You know lua? name every metamethod - skids of v3rm'+(8328-0x105c)))==2691 do __[_[__l_]]=(_[_l_l]~=0);break end;break;end break;end break;end while 1199==(_l)/((5214-(2756+-0x7e)))do _l=(4890708)while(0x95d/(191+-0x32))>=_l_ do _l-= _l _l=(5327256)while _l_<=(-0x48+87)do _l-= _l if(__[_[___l]]==__[_[_lll_]])then _ll=_ll+_lll;else _ll=_[__l_l];end;break;end while 1496==(_l)/(((631136/0xb0)+-#'1 plus 1 doesnt equal 111'))do _l=(2246630)while((111+-0x5b)+-#"porn")<_l_ do _l-= _l do return end;break end while 1769==(_l)/((0xa6a-1396))do local _l=_[__l_]__[_l](___l_(__,_l+_lll,_[_llll]))break end;break;end break;end while(_l)/(((2757-0x593)+-#"Me when moonsec:"))==3722 do _l=(5108796)while _l_<=(0x6d2/97)do _l-= _l __[_[_ll_]]=__[_[_l_l]][__[_[__llll]]];break;end while 3686==(_l)/((2810-0x590))do _l=(4328390)while _l_>(-#'staymad'+(-0x21+59))do _l-= _l __[_[__lll]]=__[_[_l__]];break end while 3610==(_l)/((0x4641/15))do __[_[_l__l]]={};break end;break;end break;end break;end break;end break;end while 2877==(_l)/((193765/0x8f))do _l=(1289848)while(130-0x63)>=_l_ do _l-= _l _l=(5648104)while _l_<=(-#"Lies"+(0xb7-154))do _l-= _l _l=(7249338)while _l_<=(2728/0x7c)do _l-= _l _l=(929838)while _l_>(0xcb7/155)do _l-= _l _ll=_[____];break end while 338==(_l)/((-#'psu more like psshit hahahaha laugh at my joke everyone'+(-0x3b+2865)))do local _ll=_[_l_l];local _l=__[_ll]for _=_ll+1,_[_lll_]do _l=_l..__[_];end;__[_[__lll]]=_l;break end;break;end while 1971==(_l)/(((7458-0xebd)+-#"staymad"))do _l=(5812101)while _l_<=(0x6b-84)do _l-= _l do return end;break;end while(_l)/((0x1e79-3934))==1503 do _l=(11635610)while _l_>(3408/0x8e)do _l-= _l local _l=_[_l__l];local __l=__[_l]local _l_=__[_l+2];if(_l_>0)then if(__l>__[_l+1])then _ll=_[_ll_l];else __[_l+3]=__l;end elseif(__l<__[_l+1])then _ll=_[_l_l];else __[_l+3]=__l;end break end while(_l)/(((0xfba+-25)+-#"go ahead. replace loadstring with dump. do it."))==2942 do local _l=_[_ll_]__[_l]=__[_l](___l_(__,_l+__l,_[_ll_l]))break end;break;end break;end break;end while 4081==(_l)/(((0x2ce74/131)+-#"no i legit burned it"))do _l=(10329330)while _l_<=(6692/0xef)do _l-= _l _l=(8457328)while(-#"I assure you officer she was a 3000 year old dragon I saw it in those japanese cartoons"+(283-0xaa))>=_l_ do _l-= _l __[_[___ll]][__[_[__l_l]]]=__[_[__ll_]];break;end while 2552==(_l)/((0x1a38-3398))do _l=(11362289)while(94-0x43)<_l_ do _l-= _l local _ll__;local _l_;local _ll_l;local _l;__[_[___ll]]=_l_ll[_[_l__]];_ll=_ll+__l;_=___[_ll];__[_[___l]]=__[_[_l_l]][_[_lll_]];_ll=_ll+__l;_=___[_ll];_l=_[__l_];_ll_l=__[_[____]];__[_l+1]=_ll_l;__[_l]=_ll_l[_[_l_l_]];_ll=_ll+__l;_=___[_ll];__[_[___ll]]=__[_[__l_l]];_ll=_ll+__l;_=___[_ll];__[_[__l_]]=__[_[_l__]];_ll=_ll+__l;_=___[_ll];_l=_[___ll]__[_l]=__[_l](___l_(__,_l+__l,_[_llll]))_ll=_ll+__l;_=___[_ll];_l=_[__lll];_ll_l=__[_[_llll]];__[_l+1]=_ll_l;__[_l]=_ll_l[_[_lll_]];_ll=_ll+__l;_=___[_ll];_l=_[_ll_]__[_l]=__[_l](__[_l+_lll])_ll=_ll+__l;_=___[_ll];_l_={__,_};_l_[_lll][_l_[__ll][___ll]]=_l_[__l][_l_[__ll][____l]]+_l_[_lll][_l_[__ll][_llll]];_ll=_ll+__l;_=___[_ll];__[_[__l_]]=__[_[_l_l]]%_[____l];_ll=_ll+__l;_=___[_ll];_l=_[_ll_]__[_l]=__[_l](__[_l+_lll])_ll=_ll+__l;_=___[_ll];_ll_l=_[____];_ll__=__[_ll_l]for _=_ll_l+1,_[_l___]do _ll__=_ll__..__[_];end;__[_[_l__l]]=_ll__;_ll=_ll+__l;_=___[_ll];_l_={__,_};_l_[_lll][_l_[__ll][___l]]=_l_[__l][_l_[__ll][_l___]]+_l_[_lll][_l_[__ll][_l__]];_ll=_ll+__l;_=___[_ll];__[_[__l_]]=__[_[_l_l]]%_[__ll_];break end while 2857==(_l)/((-116+0xffd))do local _l=_[_ll_];local _l_=__[_l+2];local __l=__[_l]+_l_;__[_l]=__l;if(_l_>0)then if(__l<=__[_l+1])then _ll=_[_l__];__[_l+3]=__l;end elseif(__l>=__[_l+1])then _ll=_[_l_l];__[_l+3]=__l;end break end;break;end break;end while 3390==(_l)/(((0x99076/101)-3159))do _l=(1723700)while(((-74+0x168)-0xcc)+-#'Day 2 of telling federal that he spilled out his milk')>=_l_ do _l-= _l __[_[___l]]=__[_[_ll_l]][_[____l]];break;end while(_l)/((0x461+-21))==1567 do _l=(1543968)while(76-0x2e)<_l_ do _l-= _l if(__[_[___ll]]~=__[_[_l_l_]])then _ll=_ll+_lll;else _ll=_[_l_l];end;break end while 864==(_l)/((0x711+-22))do local _l=_[_ll_];local _l_=__[_l+2];local __l=__[_l]+_l_;__[_l]=__l;if(_l_>0)then if(__l<=__[_l+1])then _ll=_[_l__];__[_l+3]=__l;end elseif(__l>=__[_l+1])then _ll=_[____];__[_l+3]=__l;end break end;break;end break;end break;end break;end while(_l)/((0x39c-490))==2972 do _l=(176750)while(-#'powered by ROBLOX Corporation'+(0x32c8/200))>=_l_ do _l-= _l _l=(10018504)while(0x1e09/233)>=_l_ do _l-= _l _l=(3381722)while _l_>(98-0x42)do _l-= _l local _ll=_[_ll_];local _l=__[_[_llll]];__[_ll+1]=_l;__[_ll]=_l[_[_l_l_]];break end while 1973==(_l)/((0xdb1-1791))do _l_ll[_[____]]=__[_[__l_]];break end;break;end while 2504==(_l)/((-#'still cant find the cum?'+(-37+0xfde)))do _l=(31158)while _l_<=(4080/0x78)do _l-= _l __[_[___l]]=__[_[____]]%_[_lll_];break;end while 54==(_l)/(((1413-0x302)+-#"This file has been enchanted with uncrackable V, fuck the fuck off"))do _l=(4834860)while(161+-0x7e)<_l_ do _l-= _l __[_[_ll_]]={};break end while 1220==(_l)/((7942-0xf8b))do local _=_[_ll_]__[_](__[_+_lll])break end;break;end break;end break;end while 350==(_l)/((-0x72+619))do _l=(683774)while(-#'do you ever shut the fuck up perth'+(167+-0x5e))>=_l_ do _l-= _l _l=(1026025)while _l_<=(-#":)))))))"+((-0xb2+80)+143))do _l-= _l __[_[___ll]]=__[_[__l_l]]-__[_[_lll_]];break;end while 275==(_l)/(((347576/0x5c)+-#[[KFC tried to justify urls as fake constants LOL]]))do _l=(14274)while _l_>(-0x4d+115)do _l-= _l __[_[_ll_]]=__[_[____]]%_[_l_l_];break end while 26==(_l)/((-0x3b+608))do local _l;local _l_;local __ll,___l;local _l_l;local _l;__[_[_ll_]]=_l_ll[_[____]];_ll=_ll+__l;_=___[_ll];__[_[_ll_]]=__[_[__l_l]][_[_l___]];_ll=_ll+__l;_=___[_ll];__[_[_l__l]]=__[_[_ll_l]][_[_lll_]];_ll=_ll+__l;_=___[_ll];__[_[__lll]]=__[_[_ll_l]][_[____l]];_ll=_ll+__l;_=___[_ll];_l=_[__lll];_l_l=__[_[____]];__[_l+1]=_l_l;__[_l]=_l_l[_[_lll_]];_ll=_ll+__l;_=___[_ll];_l=_[__l_]__ll,___l=___lll(__[_l](__[_l+_lll]))__l__=___l+_l-__l _l_=0;for _=_l,__l__ do _l_=_l_+__l;__[_]=__ll[_l_];end;_ll=_ll+__l;_=___[_ll];_l=_[__l_]__ll={__[_l](___l_(__,_l+1,__l__))};_l_=0;for _=_l,_[__llll]do _l_=_l_+__l;__[_]=__ll[_l_];end _ll=_ll+__l;_=___[_ll];_ll=_[_l__];break end;break;end break;end while 1183==(_l)/((626+-0x30))do _l=(5113196)while _l_<=(-#[[perth is an illusion by perth to hide perth from perth]]+(0xf1-147))do _l-= _l local _=_[___l]__[_]=__[_](__[_+_lll])break;end while(_l)/((-#'bald'+(0xbd2-(-75+0x65a))))==3476 do _l=(310878)while(8036/0xc4)<_l_ do _l-= _l local _l_;local _l;__[_[___l]]=__[_[__l_l]][_[_l_l_]];_ll=_ll+__l;_=___[_ll];__[_[__l_]]=__[_[_l_l]][_[_l___]];_ll=_ll+__l;_=___[_ll];__[_[__lll]]=_l_ll[_[__l_l]];_ll=_ll+__l;_=___[_ll];__[_[__lll]]=__[_[_llll]][_[__llll]];_ll=_ll+__l;_=___[_ll];__[_[___l]]=__[_[_ll_l]][_[_l_l_]];_ll=_ll+__l;_=___[_ll];__[_[__l_]]=__[_[_l__]][_[____l]];_ll=_ll+__l;_=___[_ll];__[_[_ll_]]=__[_[____]][__[_[__ll_]]];_ll=_ll+__l;_=___[_ll];__[_[___ll]][_[_ll_l]]=__[_[_l___]];_ll=_ll+__l;_=___[_ll];_l=_[___ll];_l_=__[_[_l_l]];__[_l+1]=_l_;__[_l]=_l_[_[_l___]];_ll=_ll+__l;_=___[_ll];_l=_[___l]__[_l](__[_l+_lll])_ll=_ll+__l;_=___[_ll];_l=_[__lll];_l_=__[_[_l__]];__[_l+1]=_l_;__[_l]=_l_[_[____l]];_ll=_ll+__l;_=___[_ll];_l=_[_ll_]__[_l](__[_l+_lll])_ll=_ll+__l;_=___[_ll];__[_[_l__l]]=_l_ll[_[_ll_l]];_ll=_ll+__l;_=___[_ll];__[_[___l]]();_ll=_ll+__l;_=___[_ll];__[_[___l]]=_l_ll[_[_ll_l]];_ll=_ll+__l;_=___[_ll];__[_[__l_]]=__[_[_llll]][_[____l]];_ll=_ll+__l;_=___[_ll];__[_[___l]]=__[_[__l_l]][_[__ll_]];_ll=_ll+__l;_=___[_ll];__[_[___l]]=__[_[____]][_[_lll_]];_ll=_ll+__l;_=___[_ll];__[_[___ll]][_[____]]=__[_[__ll_]];break end while(_l)/((767-0x1a9))==909 do __[_[__lll]]=(_[_l_l]~=0);break end;break;end break;end break;end break;end break;end break;end while 3730==(_l)/((659-(833-0x1b8)))do _l=(2812140)while _l_<=(-#[[water is wet]]+(-0x62+173))do _l-= _l _l=(6822225)while _l_<=((0xaf+-104)+-#'Jeff Bezos approved')do _l-= _l _l=(796536)while _l_<=(0x92+-99)do _l-= _l _l=(28116)while((-77+0x89)+-#"Federal is godly")>=_l_ do _l-= _l _l=(3427272)while(0x9c-113)<_l_ do _l-= _l __[_[__l_]]=__[_[_llll]];break end while(_l)/((0xc02d6/226))==984 do local _l=_[__l_];local _ll=__[_[__l_l]];__[_l+1]=_ll;__[_l]=_ll[_[__ll_]];break end;break;end while(_l)/((0x73+-82))==852 do _l=(4118828)while _l_<=((28305/0xff)+-#'This file has been enchanted with uncrackable V, fuck the fuck off')do _l-= _l __[_[___l]]=_____(_lllll[_[__l_l]],nil,_l_ll);break;end while(_l)/(((-0x4cc8/156)+1144))==4046 do _l=(9898879)while _l_>(5520/0x78)do _l-= _l __[_[_ll_]][_[_ll_l]]=__[_[__ll_]];break end while(_l)/((0xac5b8/232))==3253 do if(__[_[__lll]]~=_[__ll_])then _ll=_ll+_lll;else _ll=_[_l_l];end;break end;break;end break;end break;end while 2664==(_l)/(((0x6f94/74)+-#'helloretard will face off against MoonSec if Federal keeps deleting my strings fuck you'))do _l=(1864464)while(-#"hint: the script is in line 1"+((-#[[This file has been enchanted with uncrackable V, fuck the fuck off]]+(0x13b+-55))-0x74))>=_l_ do _l-= _l _l=(13630335)while _l_>((23814/0xf3)+-#'Do you even know what sizeof size_t equals to Lmao')do _l-= _l __[_[_l__l]][_[_ll_l]]=__[_[__llll]];break end while 3715==(_l)/((418266/(7866/0x45)))do _ll__[_[_ll_l]]=__[_[__l_]];break end;break;end while(_l)/((-#'Lies'+(5315-0xa93)))==716 do _l=(4898775)while(-88+(0xad+-35))>=_l_ do _l-= _l __[_[__l_]][_[_llll]]=_[____l];break;end while 3225==(_l)/((3092-(-#"The Great Sage Equal To Heaven is here Luraph users hide!!!!"+(0x33080/128))))do _l=(3178092)while(0xb3-128)<_l_ do _l-= _l local _={__,_};_[_lll][_[__ll][__l_]]=_[__l][_[__ll][____l]]+_[_lll][_[__ll][_l_l]];break end while 2014==(_l)/((-0x5c+1670))do local __ll=_lllll[_[_l_l]];local _l_;local _l={};_l_=_lll_l({},{__index=function(__,_)local _=_l[_];return _[1][_[2]];end,__newindex=function(_ll,_,__)local _=_l[_]_[1][_[2]]=__;end;});for __l=1,_[__ll_]do _ll=_ll+_lll;local _=___[_ll];if _[((0xf2-181)+-#'The Great Sage Equal To Heaven is here Luraph users hide!!!!')]==44 then _l[__l-1]={__,_[_ll_l]};else _l[__l-1]={_ll__,_[_l__]};end;_l_lll[#_l_lll+1]=_l;end;__[_[__lll]]=_____(__ll,_l_,_l_ll);break end;break;end break;end break;end break;end while 2025==(_l)/((0x1a95-3436))do _l=(1237712)while _l_<=(8094/0x8e)do _l-= _l _l=(1013424)while(179+-0x7d)>=_l_ do _l-= _l _l=(109720)while(10759/0xcb)<_l_ do _l-= _l _l_ll[_[_l__]]=__[_[_ll_]];_ll=_ll+__l;_=___[_ll];__[_[___ll]]={};_ll=_ll+__l;_=___[_ll];__[_[__lll]]={};_ll=_ll+__l;_=___[_ll];_l_ll[_[_llll]]=__[_[___l]];_ll=_ll+__l;_=___[_ll];__[_[_l__l]]=_l_ll[_[_llll]];_ll=_ll+__l;_=___[_ll];if(__[_[__l_]]~=_[_l___])then _ll=_ll+_lll;else _ll=_[_l_l];end;break end while(_l)/((-83+0x25b))==211 do local _l_;local _l;_l_ll[_[__l_l]]=__[_[__lll]];_ll=_ll+__l;_=___[_ll];__[_[_ll_]]=_l_ll[_[__l_l]];_ll=_ll+__l;_=___[_ll];__[_[___l]]=_[____];_ll=_ll+__l;_=___[_ll];_l=_[__l_]__[_l](__[_l+_lll])_ll=_ll+__l;_=___[_ll];__[_[___ll]]=_l_ll[_[_llll]];_ll=_ll+__l;_=___[_ll];__[_[___ll]][_[_l_l]]=_[_l_l_];_ll=_ll+__l;_=___[_ll];__[_[__lll]]=_l_ll[_[____]];_ll=_ll+__l;_=___[_ll];_l=_[_l__l];_l_=__[_[____]];__[_l+1]=_l_;__[_l]=_l_[_[____l]];_ll=_ll+__l;_=___[_ll];__[_[___l]]=_[_ll_l];_ll=_ll+__l;_=___[_ll];_l=_[_l__l]__[_l]=__[_l](___l_(__,_l+__l,_[__l_l]))break end;break;end while 258==(_l)/((-0x29+(3991+-0x16)))do _l=(6342224)while _l_<=(5060/0x5c)do _l-= _l __[_[_l__l]]=_____(_lllll[_[_l_l]],nil,_l_ll);break;end while(_l)/((-85+0xd58))==1904 do _l=(6351165)while((206-0x8f)+-#"hi skid")<_l_ do _l-= _l local _={__,_};_[_lll][_[__ll][__lll]]=_[__l][_[__ll][_lll_]]+_[_lll][_[__ll][____]];break end while(_l)/((0x6cdc5/119))==1695 do __[_[___ll]]=_l_ll[_[____]];break end;break;end break;end break;end while 688==(_l)/((0xe38-1841))do _l=(7434049)while(0x3480/224)>=_l_ do _l-= _l _l=(1101493)while(0xa6+-108)>=_l_ do _l-= _l _l_ll[_[_l__]]=__[_[_l__l]];break;end while(_l)/((-0x5b+668))==1909 do _l=(548064)while(0xc8-141)<_l_ do _l-= _l if __[_[_ll_]]then _ll=_ll+__l;else _ll=_[_l_l];end;break end while(_l)/(((0x190d-3230)-0x65a))==352 do __[_[_l__l]]();break end;break;end break;end while 2443==(_l)/((-108+0xc4f))do _l=(13792680)while _l_<=(175+-0x72)do _l-= _l local _=_[__l_]local _ll,_l=___lll(__[_](__[_+_lll]))__l__=_l+_-__l local _l=0;for _=_,__l__ do _l=_l+__l;__[_]=_ll[_l];end;break;end while 3870==(_l)/((-#"ligma balls"+(0x1c67-3696)))do _l=(10311588)while _l_>(-#"teefus more like pedofus"+(201-0x73))do _l-= _l if not __[_[_ll_]]then _ll=_ll+_lll;else _ll=_[_l_l];end;break end while(_l)/((555768/0xba))==3451 do local _lll;local _l_;local _l;__[_[__lll]]=_[_l__];_ll=_ll+__l;_=___[_ll];__[_[___ll]]=_[_ll_l];_ll=_ll+__l;_=___[_ll];__[_[___ll]]=#__[_[_l_l]];_ll=_ll+__l;_=___[_ll];__[_[__l_]]=_[_llll];_ll=_ll+__l;_=___[_ll];_l=_[___l];_l_=__[_l]_lll=__[_l+2];if(_lll>0)then if(_l_>__[_l+1])then _ll=_[__l_l];else __[_l+3]=_l_;end elseif(_l_<__[_l+1])then _ll=_[__l_l];else __[_l+3]=_l_;end break end;break;end break;end break;end break;end break;end while(_l)/((0xb715/51))==3060 do _l=(8640834)while _l_<=(0x87+-61)do _l-= _l _l=(2733159)while(157-0x59)>=_l_ do _l-= _l _l=(5976740)while _l_<=((-48+0x97)+-#'Broo u/thatHEXdude slapped this server')do _l-= _l _l=(6576534)while(-119+0xb7)<_l_ do _l-= _l __[_[__l_]]=_ll__[_[_ll_l]];break end while(_l)/((-0x47+2564))==2638 do __[_[_l__l]]=_[____];break end;break;end while(_l)/((0x630+-44))==3881 do _l=(1593558)while _l_<=(-#"someone play kogama with perth please hes so lonely"+(303-0xba))do _l-= _l local _l_=_lllll[_[_llll]];local __l;local _l={};__l=_lll_l({},{__index=function(__,_)local _=_l[_];return _[1][_[2]];end,__newindex=function(_ll,_,__)local _=_l[_]_[1][_[2]]=__;end;});for __l=1,_[__llll]do _ll=_ll+_lll;local _=___[_ll];if _[(0x66-101)]==44 then _l[__l-1]={__,_[_llll]};else _l[__l-1]={_ll__,_[_l__]};end;_l_lll[#_l_lll+1]=_l;end;__[_[__l_]]=_____(_l_,__l,_l_ll);break;end while(_l)/(((2526-0x515)+-#'oh wait thats an invalid character'))==1338 do _l=(10682208)while _l_>(-#[[This file has been enchanted with uncrackable V, fuck the fuck off]]+(-25+0x9e))do _l-= _l local _l=_[__l_]local _l_={__[_l](___l_(__,_l+1,__l__))};local _ll=0;for _=_l,_[__ll_]do _ll=_ll+__l;__[_]=_l_[_ll];end break end while(_l)/(((-#'while true do end'+(0x12fca0/220))-2855))==3837 do __[_[___l]][__[_[_l_l]]]=__[_[_l_l_]];break end;break;end break;end break;end while 3289==(_l)/(((0x4b320/176)-919))do _l=(1387161)while _l_<=((128+-0x2d)+-#"i love perth")do _l-= _l _l=(6943)while _l_<=((17808/0x70)+-#'I have enchanted this script with uncrackable V, your only option is to fuck the fuck off.')do _l-= _l __[_[___l]]();break;end while 131==(_l)/(((5994/0x51)+-#"Shard fard poo gaymer"))do _l=(607848)while _l_>((23760/0xa5)+-#[[Arse Bloody Bugger Cow Crap Damn Ginger Git God Goddam Jesus Christ Minger]])do _l-= _l if(__[_[_ll_]]~=__[_[__llll]])then _ll=_ll+_lll;else _ll=_[_l_l];end;break end while(_l)/((339+-0x51))==2356 do local _l=_[_l__l];local __l=__[_l]local _l_=__[_l+2];if(_l_>0)then if(__l>__[_l+1])then _ll=_[_l__];else __[_l+3]=__l;end elseif(__l<__[_l+1])then _ll=_[_l_l];else __[_l+3]=__l;end break end;break;end break;end while 1951==(_l)/((1521-0x32a))do _l=(621432)while(-66+0x8a)>=_l_ do _l-= _l __[_[_ll_]]=#__[_[_l_l]];break;end while(_l)/((18900/0x4b))==2466 do _l=(4395309)while _l_>(224-0x97)do _l-= _l local _=_[_ll_]local _ll,_l=___lll(__[_](__[_+_lll]))__l__=_l+_-__l local _l=0;for _=_,__l__ do _l=_l+__l;__[_]=_ll[_l];end;break end while(_l)/(((-91+0x701)+-#"<@!761654159095103499> shut the fuck up"))==2643 do local _l_=_[___ll];local ___=_[_l_l_];local _l=_l_+2 local _l_={__[_l_](__[_l_+1],__[_l])};for _=1,___ do __[_l+_]=_l_[_];end;local _l_=_l_[1]if _l_ then __[_l]=_l_ _ll=_[_llll];else _ll=_ll+__l;end;break end;break;end break;end break;end break;end while 3414==(_l)/(((332085/0x83)+-#[[Nigh]]))do _l=(2042838)while(-0x12+97)>=_l_ do _l-= _l _l=(2099776)while(138+-0x3e)>=_l_ do _l-= _l _l=(1223334)while(-48+0x7b)<_l_ do _l-= _l local _l=_[___ll]local _l_={__[_l](___l_(__,_l+1,__l__))};local _ll=0;for _=_l,_[_lll_]do _ll=_ll+__l;__[_]=_l_[_ll];end break end while 1387==(_l)/((-#'midruto'+(-25+0x392)))do if __[_[___l]]then _ll=_ll+__l;else _ll=_[_l_l];end;break end;break;end while(_l)/((0x532-728))==3488 do _l=(3518655)while _l_<=((0x83+-19)+-#[[stop looking at me im showering smh]])do _l-= _l __[_[_ll_]]=_l_ll[_[_ll_l]];break;end while(_l)/((-#[[How to dump moonsec]]+(-0x57+2521)))==1457 do _l=(8325747)while(16380/0xd2)<_l_ do _l-= _l local _=_[__l_]__[_](__[_+_lll])break end while 2943==(_l)/(((0x16b3-(-#'POV New owners'+(596000/0xc8)))+-#"follow your nose"))do local _l=_[_l__l]__[_l](___l_(__,_l+_lll,_[_l__]))break end;break;end break;end break;end while(_l)/(((-23+0x25a)+-#'Shard fard poo gaymer'))==3661 do _l=(6721814)while(0xf9-167)>=_l_ do _l-= _l _l=(9540784)while _l_<=(-0x78+200)do _l-= _l do return __[_[_l__l]]end break;end while(_l)/(((0x6b637/151)+-#'This script was obfuscated with luasecure'))==3322 do _l=(7014540)while _l_>(0x103-178)do _l-= _l local _l=_[_ll_]__[_l]=__[_l](___l_(__,_l+__l,_[____]))break end while(_l)/(((6449-0xcc4)+-#"True af"))==2210 do __[_[___l]]=__[_[_ll_l]]-__[_[____l]];break end;break;end break;end while(_l)/((1984+(-#"Ok federal give us MSv3 when"+(306/0x99))))==3433 do _l=(11983344)while(0xd2+-127)>=_l_ do _l-= _l local _ll=_[_l__];local _l=__[_ll]for _=_ll+1,_[_lll_]do _l=_l..__[_];end;__[_[___l]]=_l;break;end while(_l)/((-#'Searching for the wrapper function'+(0x6bf94/130)))==3558 do _l=(129066)while _l_>(-#'win+L = solution'+(-78+0xb2))do _l-= _l do return __[_[___l]]end break end while(_l)/((0xa1ee/141))==439 do __[_[__l_]]=(_[____]~=0);_ll=_ll+_lll;break end;break;end break;end break;end break;end break;end break;end _ll+= _lll end;end);end;return _____(_ll_ll(),{},__l__l())()end)_msec({[(245+-0x43)]='\115\116'..(function(_)return(_ and'㒘㒠㒝㒛㒣㒘㒣㒣㒦㒦㒦')or'\114\105'or'\120\58'end)((-118+(10947/0x59))==(-0x17+29))..'\110g',["㒤㒥㒞㒛㒚㒚㒥㒙㒚㒥"]='\108\100'..(function(_)return(_ and'㒥㒥㒠㒥㒡㒡㒝㒦㒚㒣㒠㒜㒣㒠㒦㒞㒛㒣')or'\101\120'or'\119\111'end)((0x5f+-90)==(-#'big harry black guy nuts'+(-0x46+100)))..'\112',["㒘㒚㒢㒘㒛㒗㒗㒛㒛"]=(function(_)return(_ and'㒦㒟㒗㒤㒞㒦㒝㒣㒥㒢㒤㒛㒤㒙')and'\98\121'or'\100\120'end)((1265/0xfd)==(128+-0x7b))..'\116\101',["㒝㒡㒞㒤㒜㒤㒚㒜㒝㒡㒡㒥㒞㒥㒙㒤"]='\99'..(function(_)return(_ and'㒟㒚㒣㒤㒙㒘㒟㒗㒥㒛㒦㒞㒘')and'\90\19\157'or'\104\97'end)((-94+0x63)==(0x2d-42))..'\114',[(-0x5c+681)]='\116\97'..(function(_)return(_ and'㒢㒥㒟㒘㒥㒡㒚㒛㒙㒦㒟㒗㒟㒠')and'\64\113'or'\98\108'end)(((0x30-36)+-#[[hacker]])==(0x46/14))..'\101',["㒘㒥㒛㒥㒛㒘㒝㒛"]=(function(_)return(_ and'㒜㒛㒛㒛㒢㒝㒜㒢㒠㒦㒜㒦㒥')or'\115\117'or'\78\107'end)((0x64-97)==(0x5b-60))..'\98',["㒛㒙㒗㒛㒝㒠㒞㒢㒞㒛㒢㒠㒡㒜"]='\99\111'..(function(_)return(_ and'㒛㒝㒗㒟㒛㒤㒦㒚㒥㒣㒡㒚㒣㒤㒙㒗㒤')and'\110\99'or'\110\105\103\97'end)((0x78+(-#'// rip gmod users'+(-15768/0xdb)))==(-#[[perth is an illusion by perth to hide perth from perth]]+(133+-0x30)))..'\97\116',[((2869760/0x26)/0x76)]=(function(_,_l)return(_ and'㒡㒥㒤㒙㒜㒘㒘㒗㒚㒠㒥㒦㒚㒝㒙㒢㒡㒡㒗')and'\48\159\158\188\10'or'\109\97'end)((102-0x61)==(47-0x29))..'\116\104',[(((-0x2e+293178)/0xcb)+-#[[psst.. change all returns to dump to get the source code]])]=(function(_,_l)return((31-(0x93+-121))==(453/0x97)and'\48'..'\195'or _..((not'\20\95\69'and'\90'..'\180'or _l)))or'\199\203\95'end),["㒟㒛㒙㒙㒢㒜㒦㒛㒛㒚"]='\105\110'..(function(_,_l)return(_ and'㒗㒚㒠㒘㒛㒡㒢㒗㒗㒡㒥㒗㒙㒝㒤㒜㒡㒝㒤')and'\90\115\138\115\15'or'\115\101'end)((-#"oh, i forgot i can write some shit here so ya dummies will see it"+(0x31c4/182))==(0x59-58))..'\114\116',["㒦㒝㒝㒦㒘㒚㒣㒞㒡"]='\117\110'..(function(_,_l)return(_ and'㒞㒡㒞㒝㒣㒞㒣㒝㒗㒠㒗㒝㒞')or'\112\97'or'\20\38\154'end)((480/0x60)==(0x60-65))..'\99\107',["㒟㒡㒗㒣㒤㒞㒢㒞㒠㒡㒘"]='\115\101'..(function(_)return(_ and'㒝㒦㒜㒡㒡㒟㒝㒙㒡㒥㒙㒥')and'\110\112\99\104'or'\108\101'end)((0x46-65)==(2046/0x42))..'\99\116',["㒟㒛㒚㒙㒢㒦㒗㒢㒞㒥㒥㒦"]='\116\111\110'..(function(_,_l)return(_ and'㒦㒘㒥㒘㒦㒥㒛㒙㒢㒦㒜㒞㒞㒢㒝㒘')and'\117\109\98'or'\100\97\120\122'end)((-#[[control c, control v]]+(((6400+-0x12)+-#'Oh so you know C++? What does sizeof(int) equal to? (gcc)')/253))==((-0x20+77)+-#'Found an xxxxxxxxxl store for ur fat mom'))..'\101\114'},{["㒞㒙㒡㒣㒞㒙㒢㒞㒡㒗㒤㒥㒝㒞"]=((getfenv))},((getfenv))()) end)()
        end)



		--Charapterr


	local Main = Window:NewTab("Character")
    local CharapterSection = Main:NewSection("Character")


    CharapterSection:NewButton("Beerus Animation", "Use Beerus Animation", function()
        if not game:IsLoaded() then
            game.Loaded:Wait()
            end wait()
            
            player = game.Players.LocalPlayer while wait() do
            if game.Workspace.Live[player.Name].Animate.idle:FindFirstChild("Animation1") then
            game.Workspace.Live[player.Name].Animate.idle:FindFirstChild("Animation1").AnimationId = "rbxassetid://1171558651"
            if game.Workspace.Live[player.Name].Animate.walk:FindFirstChild("RunAnim") then
            game.Workspace.Live[player.Name].Animate.walk:FindFirstChild("RunAnim").AnimationId = "rbxassetid://1171558651"
            end end end
	end)


	CharapterSection:NewButton("Hide Level", "Hide your Level", function()
		if not game:IsLoaded() then
			game.Loaded:Wait()
			end
			wait(2)
			game.Players.LocalPlayer.Character:FindFirstChildOfClass("Model"):Destroy()
	end)


    CharapterSection:NewButton("Hide Wings", "Hide Wings", function()
        

getgenv().enabler = true  


if (not game:IsLoaded()) then
    game.Loaded:Wait();
end;
local lplr=game:GetService('Players').LocalPlayer;
local char=game:GetService('Workspace'):waitForChild('Live'):waitForChild(lplr.Name);
function xd(char)
    lmfao=false;
    if (getgenv().enabler==false) then
        ran:Disconnect();
    else
        repeat wait();
            if (char:findFirstChild('RebirthWings')) then
                x=char.HumanoidRootPart.CFrame.X;
                y=char.HumanoidRootPart.CFrame.Y;
                z=char.HumanoidRootPart.CFrame.Z;
                char.HumanoidRootPart.CFrame=CFrame.new(x,y,z) + Vector3.new(0,-200,0);
                char.RebirthWings.Handle.AccessoryWeld:Destroy();
                char.HumanoidRootPart.CFrame=CFrame.new(x,y,z);
                x,y,z=nil;
                char.RebirthWings:Destroy();
                lmfao=true;
            end;
            if (char:findFirstChild('RealHalo')) then
                x=char.HumanoidRootPart.CFrame.X;
                y=char.HumanoidRootPart.CFrame.Y;
                z=char.HumanoidRootPart.CFrame.Z;
                char.HumanoidRootPart.CFrame=CFrame.new(x,y,z) + Vector3.new(0,-200,0);
                char.RealHalo.Handle.AccessoryWeld:Destroy();
                char.HumanoidRootPart.CFrame=CFrame.new(x,y,z);
                x,y,z=nil;
                char.RealHalo:Destroy();
                lmfao=true;
            end;
        until lmfao==true or getgenv().enabler==false;
    end;
end;
repeat wait()
    for i,v in pairs(char:getChildren()) do
        if v:IsA('Model') then
            lmao=true;
            xd(char);
            break;
        end;
    end;
until lmao==true;
lmao=false;
lplr.CharacterRemoving:connect(function() lmfao=true;end);
lplr.CharacterAdded:connect(function(v)
    char=v;
    xd(char);
    print('reconnected');
end);
    end)







	--respawnnn

	local Main = Window:NewTab("Respawn")
    local RespawnSection = Main:NewSection("Respawn")



	RespawnSection:NewKeybind("Fast Reset", "Press L", Enum.KeyCode.L, function()
        	-- Script generated by SimpleSpy - credits to exx#9394

	local args = {
		[1] = workspace.FriendlyNPCs:FindFirstChild("Hair Stylist")
	}

	game:GetService("Players").LocalPlayer.Backpack.ServerTraits.ChatStart:FireServer(unpack(args))
	-- Script generated by SimpleSpy - credits to exx#9394
	wait(.3)
	local args = {
		[1] = {
			[1] = "Yes"
		}
	}

	game:GetService("Players").LocalPlayer.Backpack.ServerTraits.ChatAdvance:FireServer(unpack(args))
	wait(.3)
	-- Script generated by SimpleSpy - credits to exx#9394

	local args = {
		[1] = "woah"
	}

	game:GetService("Players").LocalPlayer.Backpack.HairScript.RemoteEvent:FireServer(unpack(args))
	end)



    RespawnSection:NewKeybind("Hard Reset", "Press N", Enum.KeyCode.N, function()
        local Player = game:GetService("Players").LocalPlayer
        local Mouse = Player:GetMouse()
        
               Player.Character.Humanoid.Health = 0
	end)

    RespawnSection:NewKeybind("Rejoin", "Press AltGr", Enum.KeyCode.RightAlt, function()
        local place = game.PlaceId
        wait(0.1)
        game:GetService("TeleportService"):Teleport(place)
	end)


	--ANTI SCRIPT


	local Main = Window:NewTab("Anti Script")
    local AntiSection = Main:NewSection("Anti Script")


	AntiSection:NewButton("Anti Glich", "Anti Glich", function()
		if not game:IsLoaded() then
			game.Loaded:Wait()
			end
			
			local plr = game.Players.LocalPlayer
			
			while wait() do
				pcall(function()
					game:GetService("Workspace").Live[plr.Name].LowerTorso.BodyVelocity:Destroy()
				end)
			end
	end)




    AntiSection:NewButton("Anti Afk", "Va'mancia sta zit", function()
        wait(0.5)local ba=Instance.new("ScreenGui")
	local ca=Instance.new("TextLabel")local da=Instance.new("Frame")
	local _b=Instance.new("TextLabel")local ab=Instance.new("TextLabel")ba.Parent=game.CoreGui
	ba.ZIndexBehavior=Enum.ZIndexBehavior.Sibling;ca.Parent=ba;ca.Active=true
	ca.BackgroundColor3=Color3.new(0.176471,0.176471,0.176471)ca.Draggable=true
	ca.Position=UDim2.new(0.698610067,0,0.098096624,0)ca.Size=UDim2.new(0,370,0,52)
	ca.Font=Enum.Font.SourceSansSemibold;ca.Text="Anti AFK Script"ca.TextColor3=Color3.new(0,1,1)
	ca.TextSize=22;da.Parent=ca
	da.BackgroundColor3=Color3.new(0.196078,0.196078,0.196078)da.Position=UDim2.new(0,0,1.0192306,0)
	da.Size=UDim2.new(0,370,0,107)_b.Parent=da
	_b.BackgroundColor3=Color3.new(0.176471,0.176471,0.176471)_b.Position=UDim2.new(0,0,0.800455689,0)
	_b.Size=UDim2.new(0,370,0,21)_b.Font=Enum.Font.Arial;_b.Text="Made by Dynamic. (please subscribe)"
	_b.TextColor3=Color3.new(0,1,1)_b.TextSize=20;ab.Parent=da
	ab.BackgroundColor3=Color3.new(0.176471,0.176471,0.176471)ab.Position=UDim2.new(0,0,0.158377,0)
	ab.Size=UDim2.new(0,370,0,44)ab.Font=Enum.Font.ArialBold;ab.Text="Status: Active"
	ab.TextColor3=Color3.new(0,1,1)ab.TextSize=20;local bb=game:service'VirtualUser'
	game:service'Players'.LocalPlayer.Idled:connect(function()
		bb:CaptureController()bb:ClickButton2(Vector2.new())
		ab.Text="Roblox Tried to kick you but we didnt let them kick you :D"wait(2)ab.Text="Status : Active"end)
    end)

    AntiSection:NewButton("Anti Kick", "Anti kick", function()
        if not game:IsLoaded() then game.Loaded:Wait() end

local FinalStandTable = {536102540, 569994010, 2050207304, 882399924, 2046990924, 478132461, 3552157537, 2651456105, 3565304751, 535527772, 882375367, 3552158750}

if not table.find(FinalStandTable, game.PlaceId) then return end
game:WaitForChild("CoreGui")
game.CoreGui:WaitForChild("RobloxPromptGui")
game.CoreGui.RobloxPromptGui:WaitForChild("promptOverlay")
_G.xd = true 
while _G.xd do wait()
if game:GetService("CoreGui").RobloxPromptGui.promptOverlay:FindFirstChild("ErrorPrompt") then 
game:GetService("TeleportService"):Teleport(536102540, LocalPlayer)
end
end
    end)

    local Main = Window:NewTab("Teleport")
    local Tp5Section = Main:NewSection("City")
    
    Tp5Section:NewButton("South City", "Tp South City", function()
		game:GetService("TweenService"):Create(
           game.Players.LocalPlayer.Character.HumanoidRootPart,
           TweenInfo.new(1.2, Enum.EasingStyle.Linear, Enum.EasingDirection.Out),
           {CFrame = CFrame.new(-456, 28, -6412)}
           ):Play()
	end)

    Tp5Section:NewButton("West City", "Tp West City", function()
        game:GetService("TweenService"):Create(
           game.Players.LocalPlayer.Character.HumanoidRootPart,
           TweenInfo.new(1.2, Enum.EasingStyle.Linear, Enum.EasingDirection.Out),
           {CFrame = CFrame.new(-570, 23, -2884)}
           ):Play()
	end)

    Tp5Section:NewButton("Central City", "Tp Central City", function()
        game:GetService("TweenService"):Create(
           game.Players.LocalPlayer.Character.HumanoidRootPart,
           TweenInfo.new(1.2, Enum.EasingStyle.Linear, Enum.EasingDirection.Out),
           {CFrame = CFrame.new(-3834, 23, -1428)}
           ):Play()
	end)

    Tp5Section:NewButton("Tower", "Tp to Tower", function()
        game:GetService("TweenService"):Create(
           game.Players.LocalPlayer.Character.HumanoidRootPart,
           TweenInfo.new(1.2, Enum.EasingStyle.Linear, Enum.EasingDirection.Out),
           {CFrame = CFrame.new(2071, 1495, -2279)}
           ):Play()
	end)

    local Tp6Section = Main:NewSection("Dimension")

    Tp6Section:NewButton("Earth", "Tp to Earth", function()
        game:GetService("TeleportService"):Teleport(536102540)
	end)

    Tp6Section:NewButton("Namek", "Tp to Namek", function()
        game:GetService("TeleportService"):Teleport(882399924)
	end)

    Tp6Section:NewButton("Space", "Tp to Space", function()
        game:GetService("TeleportService"):Teleport(478132461)
	end)

    Tp6Section:NewButton("Future", "Tp to Future", function()
        game:GetService("TeleportService"):Teleport(569994010)
	end)

    Tp6Section:NewButton("Secret World", "Tp to Secret World", function()
        game:GetService("TeleportService"):Teleport(2046990924)
	end)

    Tp6Section:NewButton("Zaros", "Tp to Zaros", function()
        game:GetService("TeleportService"):Teleport(2651456105)
	end)

    Tp6Section:NewButton("Queue", "Tp to Queue", function()
        game:GetService("TeleportService"):Teleport(3565304751)
	end)

    Tp6Section:NewButton("Heaven", "Tp to Heaven", function()
        game:GetService("TeleportService"):Teleport(3552157537)
	end)



	







	local Main = Window:NewTab("Old version")
    local OldSection = Main:NewSection("Prove old Version")

    --old ver


	OldSection:NewButton("1tsJusthub v1(DBZ FS)", "prove 1tsJusthub v1(DBZ FS)", function()
		loadstring(game:HttpGet(("https://raw.githubusercontent.com/gp1tsJust/Dbz/main/README.md"), true))()
	end)


	--Credit

	local Main = Window:NewTab("Credit")
    local CreditSection = Main:NewSection("Credit to 1tsJustgp")

	local DsSection = Main:NewSection("Discord private gp1tsJust#3203")
	local DserverSection = Main:NewSection("Server Discord https://discord.gg/5xp4yx9PJN")

    DserverSection:NewButton("Copy link", "Copy link Ds server", function()
        setclipboard("https://discord.gg/5xp4yx9PJN")
    end)

    local Main = Window:NewTab("Info")
    local InfoSection = Main:NewSection("Info")
    local SoonSection = Main:NewSection("1tsJustHub V3 Soon...")



    InfoSection:NewKeybind("Hide UI", "Hide UI", Enum.KeyCode.RightControl, function()
		Library:ToggleUI()
	end)



    
