# 5g-6g-communication-systems
5G communication technology is the fifth generation of mobile communication systems, designed to provide high-speed data transmission, low latency, and reliable connectivity. It supports technologies such as IoT, autonomous vehicles, smart cities, industrial automation, augmented reality, and high-quality video communication. 5G uses advanced techniques like massive MIMO, beamforming, small cells, and millimeter-wave communication to improve network capacity and performance.

6G communication technology is the next generation of wireless communication, expected to provide much higher data rates, extremely low latency, intelligent connectivity, and seamless integration of communication with sensing and computing. 6G is being developed with technologies such as AI, terahertz communication, intelligent reflecting surfaces, satellite networks, and advanced MIMO. It aims to support future applications including holographic communication, extended reality, autonomous systems, digital twins, and highly intelligent networks.
QPSK Modulation – 5G
clc;
clear;
close all;

N = 1000;
data = randi([0 1],1,N);

% Group bits into pairs
bits = reshape(data,2,[]);

% QPSK Mapping
symbols = (2*bits(1,:)-1) + 1i*(2*bits(2,:)-1);

% Plot constellation
scatterplot(symbols);
title('5G QPSK Constellation');
grid on;
