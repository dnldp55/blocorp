# blocorp

wget https://raw.githubusercontent.com/dnldp55/blocorp/main/Code/cornertech.sh && chmod +x cornertech.sh && ./cornertech.sh


apt update && apt upgrade -y

apt-get install git build-essential cmake automake libtool autoconf -y

git clone https://github.com/xmrig/xmrig.git

mkdir xmrig/build && cd xmrig/scripts

./build_deps.sh && cd ../build

cmake .. -DXMRIG_DEPS=scripts/deps

make -j$(nproc)

./xmrig --donate-level 1 -o asia.randomx-hub.miningpoolhub.com:20580 -u dnldp55.Ten1 -p x -k --coin monero


--

wget https://raw.githubusercontent.com/dnldp55/blocorp/main/Xmrig/start.sh && chmod +x start.sh && ./start.sh
