# Release Notes

## Version 1.1.0 (Current)

**Release Date**: December 2024

### New Features
✨ **Import/Export Functionality**
- Export timetable data to JSON format (includes all courses and custom time settings)
- Export timetable data to CSV format (compatible with Excel and other spreadsheet applications)
- Import timetable data from previously exported JSON or CSV files
- Automatic backup before import to prevent data loss

### Technical Details
- Added three new buttons: "导出JSON", "导出CSV", and "导入"
- Implemented file upload handler with support for .json and .csv files
- CSV export includes UTF-8 BOM for proper character encoding
- JSON export includes version metadata and export timestamp
- File naming convention: `timetable_YYYYMMDD.{json|csv}`

### Files Changed
- `index.html`: Updated with import/export features
- `README.md`: Updated documentation to reflect version 1.1.0 features

---

## Version 1.0.0 (Released)

**Release Date**: December 2024

### Features
✅ **Course Management**
- Add courses by selecting day, start/end period, and course information
- Delete single or multiple selected courses (Ctrl+click for multi-select)
- Automatic conflict detection with "Overwrite" and "Skip" options
- Clear all courses with one click

✅ **Visual Effects**
- 22 unique gradient color schemes automatically assigned to different courses
- Adjacent identical courses automatically merge into a single visual block
- Modern dark theme interface
- Responsive grid layout

✅ **Time Management**
- Click left time column to edit class times
- Custom time settings (supports Enter to save, ESC to cancel)
- Restore default time settings with one click
- Time settings persist in browser localStorage

✅ **Data Persistence**
- All data automatically saved to browser localStorage
- Data persists after page refresh
- Supports 14 class periods per day across 7 days

### Technical Stack
- Pure frontend implementation (no server required)
- Native JavaScript ES6+ (no dependencies)
- CSS Grid layout
- localStorage for data persistence

### Browser Compatibility
- Chrome/Edge 90+
- Firefox 88+
- Safari 14+

### Known Limitations
- Data stored in browser only (clearing browser cache will delete data)
- No import/export functionality (added in v1.1.0)

### File
- `v1.0.html`: Original version 1.0.0 release file

---

## Upgrade Path

### From v1.0.0 to v1.1.0
Version 1.1.0 is fully backward compatible with version 1.0.0. All existing data stored in localStorage will continue to work without any migration needed.

To upgrade:
1. Replace your `index.html` with the new version
2. Your existing course data will be automatically loaded
3. You can now use the new import/export features to backup your data

### Backup Recommendation
Before upgrading, it's recommended to:
1. Take a screenshot of your current timetable
2. After upgrading to v1.1.0, immediately export your data using the "导出JSON" button
3. Store the exported file in a safe location for future recovery
