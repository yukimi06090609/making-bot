require "dicordrb"

bot = Discordrb::Commands::CommandBot.new(
token: NTI0MTM0MjcyMjc4MzMxMzk1.Dvjqow.yrysRdACpBthSLjRNLwiPc2oof0,
client_id: 524134272278331395,
prefix:"/",
)

bot.command :hello do |event|
 event.send_message("hello,world.#{event.user.name}")
end

bot.run
