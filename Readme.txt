Veri_Site_Toolset Prototype

"""Original Purpose"""
# The toolset is meant to make text based verification faster
# by predownloading needed site data and removing all noise related to different sites
# meaning, leaving only unique text per page and feeding it in the same format

""" Architecture """
# Toolset consists of three script files written in Py 2.7, webdriver for chrome driving and data filesystem

# site_element_retriever:
# - makes filesystem
# - retrieves static html
# - extracts unique, visible site page text
# - translates to english
# - manages input and output files

# site_veri_gui:
# Tkinter based gui for site verification. Site is represented as Tk Notebook and page as Tabs
# - manages verification related files
# - highlights text according to added and locally saved keywords, shows highlight key coount in tab header
# - shows original or translated text