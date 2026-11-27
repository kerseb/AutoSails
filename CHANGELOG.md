## [Unreleased]

### Fixed
- NullReferenceException in `AutoSailsControlSail.Start()` for sails without a hoist winch (e.g. topsails). The controller now removes itself from such sails.
- `ArgumentOutOfRangeException` risk when a sail has no angle winch.
- Input handler ignores calls from destroyed sails.


## [1.2.3] - 2025-08-02

### Fixed 
- AutoSails prevents SailInfo from displaying the name and in/out status of halyards. All descriptions are commented out.

## [1.2.2] - 2025-07-31

### Fixed 
- Hoisted status is now determined based on the status of the hoist rope length instead set if hoisted by mod. This enables trim functionality to work correct even if sails are hoisted by player. 

## [1.2.1] - 2025-07-30

### Fixed 
- Forgot to remove the debug overlay on winches

## [1.2.0] - 2025-07-30

### Added 
- Added Issue #1, Furling Sails Automation. Sheets are adjusted properly when sails furled
- Added Issue #3, Text Feedback for Sail and Trim Commands (needs to be enabled in config)
- Added Issue #4, Make Sail and Trim States Per-Boat Rather than Global
- Added Issue #5, automatic jibe with gaffs, lateens, junksails (can be disabled in config, might not work on all ships)
 
## [1.1.0] - 2025-07-27

### Added 
- Mayor refactor, controller is now attatched to sail and not to winches. 
- Added staysail and squaresail functionality

## [1.0.1] - 2025-07-24

### Fixed 
- Only sails of the ship where the player is currently on or was last on can be controlled now. Last on only possible if currently not on any ship, i.e in water or on land.
- Only ships which are owned by player can be controlled.

## [1.0.0] - 2025-07-23

### Added
- Initial release of AutoSails mod.


