# PM2 Setup Guide

## Steps

### Install PM2
Install PM2 globally.

```bash
npm install -g pm2
```

### Start Your Application
Start your application with PM2, giving it a meaningful name.

```bash
pm2 start server.js --name "Solana-Service"
```

### Setup PM2 to Start on Boot
To ensure PM2 restarts your application on boot, run the following command:

```bash
pm2 startup
```

This will provide a command that you need to copy and paste into your terminal.

### Save the PM2 Process List
Finally, save the PM2 process list to make sure your application restarts on reboot.

```bash
pm2 save
```

And that's it! 🎉 Your application is now managed by PM2 and will restart automatically on system boot.

## Additional Tips

### Check PM2 Status
View the status of your PM2 processes at any time.

```bash
pm2 status
```

### Restart Application
Restart your application easily.

```bash
pm2 restart Solana-Service
```

### Stop Application
Stop your application if needed.

```bash
pm2 stop Solana-Service
```

Happy coding! 😃

# PM2 Uninstallation Guide

## Steps

### Stop and Delete All PM2 Processes
First, stop and delete all existing PM2 processes.

```bash
pm2 stop all
pm2 delete all
pm2 kill
```

### Uninstall PM2
Next, uninstall PM2 globally to remove all configurations.

```bash
npm uninstall -g pm2
```

### Remove PM2 Configuration Directory
Remove the PM2 configuration directory to ensure a clean setup.

```bash
rm -rf ~/.pm2
```

By following these steps, PM2 will be completely removed from your system, including its configurations and processes.
