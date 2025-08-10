# Claude ToDo List - AGNO Hash System Implementation

## 🎯 Next Session Tasks

### 1. Hornet Address System Integration
- [ ] Modify Hornet's address parsing to support AGNO format
- [ ] Implement: `AGNO_000000_0_000_0_000_0000_[hash]` as default
- [ ] Update address validation in `pkg/model/` directory
- [ ] Ensure entire 95-char string treated as single hash (not prefix+hash)

### 2. Development & Testing
- [ ] Create AGNO address generation functions
- [ ] Test with all-zero classification fields during development
- [ ] Verify DAG treats complete AGNO string as immutable hash
- [ ] Add unit tests for AGNO address parsing/validation

### 3. API Integration Prep  
- [ ] Design classification API endpoint structure
- [ ] Plan how AI/Human will assign real classification values
- [ ] Ensure API output replaces development defaults properly

### 4. Documentation Updates
- [ ] Update Hornet README with AGNO integration notes
- [ ] Document new address format in Hornet config examples
- [ ] Add AGNO examples to integration tests

## 🔐 Critical Security Requirement
**ENTIRE AGNO STRING = HASH** (prevent classification tampering)

## 📂 Key Files to Modify
- `pkg/model/` - Address structures  
- `components/` - Address processing
- Config files - Add AGNO examples

## 🎯 Current Goal
Get Hornet working with AGNO development format, then build classification API later.