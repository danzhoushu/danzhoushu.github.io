---
title: "Python: A Good Friend for RF/mmW Engineers"
excerpt: "From simulations and data analysis to visualization and automation, Python offers a wide range of capabilities that make it an excellent companion for RF/mmW engineers <br/><img src='/images/Figure_skrf.png'>"
collection: portfolio
---

or RF engineering software tools, Python offers a wide range of capabilities. One notable module is [Scikit-RF](https://scikit-rf.org/) which is a powerful tool for RF simulation, data analysis, and presentation.

Python provides various modules for different tasks in RF engineering. For data collection, two typical modules are pyvisa and pyscpi. Pyvisa and pyscpi enable communication with instruments using standard protocols like GPIB, USB, and Ethernet. 

Python modules can also handle tasks beyond RF engineering. They can drive I2C, SPI, MIPI and other serial ports, execute CMD commands, interact with web browsers, and perform database queries. This versatility allows engineers to integrate different components and streamline their workflow efficiently.

Here's an example of using Scikit-RF to plot a Smith chart based on an S2P file:

<a href="/images/Figure_skrf_smith.png">
    <img 
        src="/images/Figure_skrf_smith.png" 
    >
</a>

*Pic1: Smith Chart example*

# Example Python code

import pandas as pd

from sqlalchemy import create_engine

import skrf as rf

from skrf.data import ring_slot

from pylab import *

import matplotlib.pyplot as plt

import numpy as np

from matplotlib.ticker import (MultipleLocator, AutoMinorLocator)

import subprocess

import os

import subprocess

import time

import webbrowser

import pyvisa

import pyscpi

import pymssql

import pymysql

import odbc

plt.figure(1)

from skrf import Network, Frequency

ring_slot = Network('C:/Users/Dan/Dropbox/personal/Dan/Self_learning/python/data/ring slot.s2p')

ring_slot.plot_s_db()

plt.grid(True)

plt.minorticks_on()

plt.grid(True, which='minor', linestyle='--', linewidth=0.25, color='red')


plt.title('Python Scikit-RF demo S-Parameter plot by Dan')

legend_labels = ['S11 (dB)', 'S21 (dB)', 'S12 (dB)', 'S22 (dB)']

plt.legend(legend_labels)


plt.tick_params(which='both', width=2)

plt.tick_params(which='major', length=7)

plt.tick_params(which='minor', width=2, length=4, color='grey')


plt.figure(2)

ring_slot.plot_s_smith()

plt.title('Python Scikit-RF demo Smith Chart plot by Dan')

plt.show()

batch_file = 'C:/Users/Dan/Dropbox/personal/Dan/Self_learning/python/trial1.bat'

subprocess.Popen(['cmd', '/k', batch_file], shell=True)

webbrowser.register('chrome', None, webbrowser.BackgroundBrowser('C:\Program Files\Google\Chrome\Application\chrome.exe'))

url = 'https://danzhoushu.github.io/posts/2023/04/blog-post-1/'

webbrowser.get('chrome').open(url)

webbrowser.register('chrome', None, webbrowser.BackgroundBrowser('C:\Program Files\Google\Chrome\Application\chrome.exe'))

website_url = 'https://danzhoushu.github.io/portfolio/portfolio-11/'

chrome_path = r'C:\\Program Files\\Google\\Chrome\\Application\\chrome.exe'

subprocess.Popen([chrome_path, website_url])

time.sleep(15)

subprocess.Popen(['taskkill', '/F', '/IM', 'chrome.exe'])