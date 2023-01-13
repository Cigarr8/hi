loadstring(game:HttpGet("https://pastebin.com/raw/tqf7rEBm"))();

local function callback(Text)
 if Text == "Button1 text" then
  print ("Answer")
elseif Text == ("Button2 text") then
 print ("Answer2")
 end
end

local NotificationBindable = Instance.new("BindableFunction")
NotificationBindable.OnInvoke = callback
--
game.StarterGui:SetCore("SendNotification",  {
 Title = "Commands";
 Text = "!ban, !kick, !locate ip, !headless, !faceless, !Freeze, !Unfreeze, !crash, !fov 120, !fov 60, !fov 100, !fw, !bw, !kill";
 Icon = "";
 Duration = math.huge;
 Button1 = "Close";
 Callback = NotificationBindable;
})
