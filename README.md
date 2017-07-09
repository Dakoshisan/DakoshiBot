var builder = new EmbedBuilder()
	.WithTitle("**RULES MAY BE CHANGED OR UPDATED IN FUTURE**")
	.WithDescription("1⃣ Respect the channels and their uses: Disrespect, direct harassment and Violent Behavior will result in a warning and/or kick.")
	.WithUrl("https://discordapp.com")
	.WithColor(new Color(0x25ABF8))
	.WithTimestamp(DateTimeOffset.FromUnixTimeSeconds(1499515863600))
	.WithFooter(footer => {
		footer
			.WithText("footer text")
			.WithIconUrl("https://cdn.discordapp.com/embed/avatars/0.png");
	});
	.AddField("😂", "2⃣ Do not advertise in this server or through PMs: You are not allowed to advertise your Discord server, YouTube, Twitch or anything else. This server is for friends to come together, not to make money or getting more famous.")
	.AddField("😘", "3⃣ Do not Instigate situations: If incidents occur and no admin is available, deescalate the situation. If anyone is caught egging on the incident the same action of punishment will be admitted to them as well. ")
	.AddField("🙄", "4⃣ Do not spam neither voice or text chat: Spamming voice and/or text will result with immediate mute followed by a warning. Continual spam will result with a one day ban from the discord.  ")
	.AddField("😜", "5⃣ Explicit content is to not be posted in the general chat. We have two chats to help filter out content posted in the discord, one for general members under the age of 18 and those who are 18+. If you wish to be able to post explicit content you must be given the correct role to join into the seperated chat. ")
	.AddField("<:thonkang:219069250692841473>", "are inline fields");
var embed = builder.Build();
await Context.Channel.SendMessageAsync("_", embed)
	.ConfigureAwait(false);
