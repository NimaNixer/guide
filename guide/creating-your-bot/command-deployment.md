const { REST, Routes } = require('discord.js');
const { 1111847672190599270, 1111847672190599270, MTExMTg0NzY3MjE5MDU5OTI3MA.Gi1G3X.7mk88seJ4kPWVRraGOTjRySesncxDJP9VzRBxE } = require('./config.json');

const rest = new REST().setToken(MTExMTg0NzY3MjE5MDU5OTI3MA.Gi1G3X.7mk88seJ4kPWVRraGOTjRySesncxDJP9VzRBxE);

// ...

// for guild-based commands
rest.delete(Routes.applicationGuildCommand(1111847672190599270,1111847672190599270 , 'commandId'))
	.then(() => console.log('Successfully deleted guild command'))
	.catch(console.error);

// for global commands
rest.delete(Routes.applicationCommand(1111847672190599270, 'commandId'))
	.then(() => console.log('Successfully deleted application command'))
	.catch(console.error);
