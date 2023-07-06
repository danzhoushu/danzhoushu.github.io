---
title: "Python: A Good Friend for RF/mmW Engineers"
excerpt: "From simulations and data analysis to visualization and automation, Python offers a wide range of capabilities that make it an excellent companion for RF/mmW engineers <br/><img src='/images/Figure_skrf.png'>"
collection: portfolio
---

For RF engineering software tools, we can do almost everything by Python. [Scikit-RF](https://scikit-rf.org/) is a good python modules for RF simulation, data anaysis, and presentation. For data collection, pyvisa and pysicl are two typical modules to use. Of course, Python module can drive serial port, CMD commands, web brower, data base query as well.

Below is the example of S2P file smith chart plot by Scikit-RF. I also attached a piece of Python code as the examples. 


<a href="/images/Figure_skrf_smith.png">
    <img 
        src="/images/SFigure_skrf_smith.png" 
    >
</a>
*Pic1: Smith Chart example*

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


# Add labels and title
# plt.xlabel('X')
# plt.ylabel('Y')
plt.title('Python Scikit-RF demo S-Parameter plot by Dan')
# plt.draw_if_interactive()

legend_labels = ['S11 (dB)', 'S21 (dB)', 'S12 (dB)', 'S22 (dB)']
plt.legend(legend_labels)


plt.tick_params(which='both', width=2)
plt.tick_params(which='major', length=7)
plt.tick_params(which='minor', width=2, length=4, color='grey')


plt.figure(2)
ring_slot.plot_s_smith()
plt.title('Python Scikit-RF demo Smith Chart plot by Dan')
# plt.draw_if_interactive()

plt.show()


# Batch file path
batch_file = 'C:/Users/Dan/Dropbox/personal/Dan/Self_learning/python/trial1.bat'

# Open the CMD window and execute the batch file
subprocess.Popen(['cmd', '/k', batch_file], shell=True)

webbrowser.register('chrome', None, webbrowser.BackgroundBrowser('C:\Program Files\Google\Chrome\Application\chrome.exe'))

# Website URL
url = 'https://danzhoushu.github.io/posts/2023/04/blog-post-1/'

# Open the website in Google Chrome
webbrowser.get('chrome').open(url)

webbrowser.register('chrome', None, webbrowser.BackgroundBrowser('C:\Program Files\Google\Chrome\Application\chrome.exe'))

# Website URL
website_url = 'https://danzhoushu.github.io/portfolio/portfolio-11/'

chrome_path = r'C:\\Program Files\\Google\\Chrome\\Application\\chrome.exe'

# Open Chrome with the website
subprocess.Popen([chrome_path, website_url])

# Wait for some time (e.g., 5 seconds)
time.sleep(15)

# Close the Chrome browser
subprocess.Popen(['taskkill', '/F', '/IM', 'chrome.exe'])