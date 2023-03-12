# Laravel docker preset to dockerize your Laravel app

## Installation
Create a new Laravel app
```bash
laravel new your-app-name
```
Make sure you replace `your-app-name` with the name of your app.

## Setup docker
Make sure you have Docker installed on your machine. If not, you can download it from [here](https://www.docker.com/products/docker-desktop).

Clone this repository

Switch to the cloned directory and run the following command to install the preset

If you want to use any other port, you can change the port number in the Dockerfile where it says `EXPOSE 8000`. Replace `8000` with the port number you want to use.

```bash
docker build -t your-container-name .
```
Make sure you replace `your-container-name` with the name of your container. Also do not forget the `.` at the end of the command.

## Usage
To start the container, run the following command
```bash
docker run -it -p 8000:8000 your-container-name
```

To stop the container, run the following command
```bash
docker stop your-container-id
```

If you want to use any other port, you can change the port number in the command above.


You can see the Docker containers that are currently running on your system (along with their Container IDs) with:
```bash
docker ps
```

## Push to cloud

### DigitalOcean
To push your app to DigialOcean, you need to have a account with them. If you don't have one, you can create one [here](https://cloud.digitalocean.com/registrations/new).

For more information on how to push your app to DigitalOcean, you can check out this [video](https://youtu.be/tFOPjC97umw) useful video.



## Dockerize.io
Also you can check out this [article](https://dockerize.io/guides/php-laravel-guide) for more information.


## Issues
If you have any issues, please feel free to open an issue on this repository.

## License
The MIT License (MIT). Please see [License File](LICENSE.md) for more information.

## Credits
- [Laravel](https://laravel.com/)
- [Docker](https://www.docker.com/)
- [DigitalOcean](https://www.digitalocean.com/)
- [Dockerize.io](https://dockerize.io/guides/php-laravel-guide)
