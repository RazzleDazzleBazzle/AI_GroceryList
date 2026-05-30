# AI_GroceryList  
AI driven Grocery List app for iOS and iPadOS  

Privacy policy 

Information We Collect — Analytics / Crash reports submitted by end user to Apple.  
iCloud Sync — explains Apple's role, encryption, and how to disable it  
How We Use Your Information — We don't collect it.  
Data Sharing & Third Parties — Anonymised analytics only, nothing sold  
Data Retention & Deletion — user is in full control, how to delete everything  
Your Privacy Rights — access, correction, deletion, opt-out  
Children's Privacy — under-13 policy  
Security — iCloud encryption, no location logging  
Changes to This Policy — in-app notification process  
Contact Us — DarrenWilson23@icloud.com  

AI Grocery List  

A full-featured iOS grocery list manager built with SwiftUI and CloudKit, designed for solo shoppers and households alike.  

Features  

Lists & Items  
• Create multiple shopping lists, each optionally assigned to a store  
• Add items with name, quantity, unit of measure, category, aisle, notes, and photo  
• Mark items checked/unchecked with visual strikethrough  
• Group items by aisle for efficient in-store navigation  
• Rename, archive, or delete lists  
• Swipe to delete individual items  
• Wishlists — a separate list type for tracking items you want but aren't actively shopping for, with bulk-add to any shopping list  

Smart Aisle Learning  
• Automatically suggests the aisle for an item based on your past shopping history at that store  
• Prompts for an aisle when checking off an item that doesn't have one yet  
• Aisle mappings are stored per store and re-applied when switching a list's store  

Reminders  
• Set urgency levels on items: None, Low, ASAP, This Afternoon, Tonight, This Week  
• Three reminder trigger types: Date & Time, Location (geofence on arrival), or both combined  
• List-level reminders independent of individual item reminders  
• Reminders auto-cancel when an item is checked off or a shop is finished  
• Full reminder log with colour-coded events (scheduled, delivered, cancelled, failed)  

Finish Shop  
• Marks all checked items as complete and moves them to Shopping History  
• Clears list-level reminders automatically  
• Works correctly with shared (CloudKit) lists — history is distributed to all participants without duplication  

Shopping History  
• Completed items are saved with store name and date  
• Grouped by shopping trip (store + date)  
• Searchable by item name  
• Re-add any historical item to a new list in one tap  
• Deduplicates items when presenting the "Add from History" picker  

Barcode Scanning  
• Full-screen camera scanner supporting EAN-13, UPC, Code128, QR, and more  
• Looks up product names from configurable barcode databases (EAN Search, Barcode Lookup)  
• Pinch-to-zoom, tap-to-focus, and torch control during scanning  

Product Label Scanning  
• Camera view with adjustable crop region to frame a product label  
• OCR extracts text (ingredients, allergens, nutrition info) and appends it to item notes  

Recipes  
• Create recipes with ingredients (name, quantity, unit, category)  
• Import recipes directly from a URL — the app fetches and parses the page to extract ingredients automatically  
• Add all ingredients from a recipe to any shopping list in one tap  
• Share recipes from Safari via the iOS Share Extension  

Stores  
• Maintain a list of your regular stores with name, address, and map coordinates  
• Interactive map with native POI tap support and location search  
• Store coordinates enable location-based reminders and aisle learning  

Sharing & Collaboration (CloudKit)  
• Share any list with other iCloud users with read or read/write permissions  
• Changes sync in real time to all participants  
• Completed items from other participants appear in your local Shopping History  
• Stale share zone detection and cleanup  

Photos  
• Attach a photo to any item via camera, photo library, or clipboard paste  
• Full-screen photo viewer with zoom  
• Automatic image compression  

Settings  
• Manage and reorder barcode database sources, configure API keys  
• View and share finish-shop diagnostic logs  
• Clear all scheduled reminders  
• Force-stop sharing for lists with stale CloudKit metadata  

Tech Stack  

• SwiftUI — UI throughout  
• Core Data + NSPersistentCloudKitContainer — local storage and CloudKit sync  
• CloudKit — list sharing and collaborative history  
• AVFoundation — barcode and product label scanning  
• Vision — OCR for product label text extraction  
• Core Location + UserNotifications — geofence and date/time reminders  
• MapKit — store location browsing and POI search  
• App Extension — Safari Share Extension for recipe import  
