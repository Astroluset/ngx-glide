# ngx-glide v21.0.0 - Release Preparation Summary

## ✅ Completed Updates

### 📝 Documentation Updates
- ✅ Updated README.md to specify Angular 21+ support only
- ✅ Added migration guide with breaking changes
- ✅ Updated installation instructions with proper version
- ✅ Fixed build configuration examples with .scss extensions
- ✅ Added CHANGELOG entry for v21.0.0 with breaking changes

### 📦 Package Configuration
- ✅ Updated root package.json version to 21.0.0
- ✅ Updated ngx-glide package.json version to 21.0.0
- ✅ Updated peer dependencies to require Angular 21+
- ✅ Fixed build scripts for Windows compatibility
- ✅ Added npm publish scripts (dry-run and live)

### 🛠️ Technical Updates
- ✅ Fixed Sass @use imports in styles.scss
- ✅ Updated project.json with proper .scss extensions
- ✅ Updated TypeScript target to ES2022 for Angular 21
- ✅ Verified build process works correctly
- ✅ Tested npm publish dry-run successfully

## 🚀 Ready for Release

### Pre-Merge Checklist
- ✅ All documentation updated
- ✅ Version numbers bumped to 21.0.0
- ✅ Build process working
- ✅ Package can be published
- ✅ Breaking changes documented

### Merge to Master Steps
1. Commit all current changes
2. Push to feature branch
3. Create pull request to master
4. Review and merge

### NPM Publish Steps
After merging to master:

```bash
# Final build and publish
npm run publish:ngx-glide

# Or step by step:
npm run build:ngx-glide
cd dist/packages/ngx-glide
npm publish
```

### Publishing Checklist
- [ ] Merged to master
- [ ] Tagged release v21.0.0
- [ ] Published to npm
- [ ] Verified package on npmjs.com
- [ ] Updated GitHub release notes

## 📋 Breaking Changes Summary

### What Changed
- **Angular 21+ Required**: Previous versions not supported
- **Sass @import Deprecated**: Must use @use syntax
- **Build Configuration**: Requires .scss extensions in styles array

### Migration Steps for Users
1. Upgrade to Angular 21
2. Update package: `npm install ngx-glide@21`
3. Update angular.json/project.json styles configuration
4. Replace @import with @use in custom styles (if any)

## 📊 Package Details
- **Name**: ngx-glide
- **Version**: 21.0.0
- **Size**: 14.4 kB packed, 70.3 kB unpacked
- **Dependencies**: @angular/core@>=21.0.0, @angular/common@>=21.0.0, @glidejs/glide@3.x
- **Repository**: https://github.com/Astroluset/ngx-glide