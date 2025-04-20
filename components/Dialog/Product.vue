<template>
	<v-card class="pa-4">
		<v-row class="pt-9 px-5">
			<v-col class="text-center">
				<span class="text-h5">{{ edit ? 'Edit' : 'Add' }} Product Information 111</span>
			</v-col>
			<v-col cols="2" class="text-right">
				<v-btn icon @click="CloseForm">
					<v-icon>mdi-close</v-icon>
				</v-btn>
			</v-col>
		</v-row>

		<v-card-text>
			<v-form v-model="isValid" ref="form" class="px-15">
				<v-row>
					<v-col cols="12">
						<v-row>
							<v-col cols="12">
								<label>product_name<span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.product_name"
									:rules="[rules.required]"
									placeholder="Enter Title"
								/>
							</v-col>

							<v-col cols="6">
								<label class="required">ingredients</label>
								<v-text-field
									outlined
									placeholder="Enter ingredients"
									:rules="[rules.required]"
									v-model="payload.ingredients"
								/>
							</v-col>

							<v-col cols="6">
								<label>weight <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.weight"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>fat <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.fat"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>protein <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.protein"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>carbohydrates <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.carbohydrates"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>energy <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.energy"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>acidity_as_citric_acid <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.acidity_as_citric_acid"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>sugar <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.sugar"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>calcium <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.calcium"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>trans_fat <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.trans_fat"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>saturated_fat <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.saturated_fat"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>sodium <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.sodium"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>total_fat <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.total_fat"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>citric_acid <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.citric_acid"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>taurine <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.taurine"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>caffeine <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.caffeine"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>inositol <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.inositol"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>niacin <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.niacin"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>vitamin_b6 <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.vitamin_b6"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>vitamin_b3 <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.vitamin_b3"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="6">
								<label>vitamin b12 <span class="red--text">*</span></label>
								<v-text-field
									outlined
									v-model="payload.vitamin_b12"
									placeholder="Enter SKU"
									:rules="[rules.required]"
								/>
							</v-col>
							<v-col cols="4">
								<v-col cols="6">
									<label>Desktop Banner<sup class="red--text">*</sup></label>
									<FormElementsFileInput
										v-model="payload.product_image"
										:errorMessage="errorMessages.product_image"
										@change="isImagesValidated(['product_image'])"
										:UploadAPI="HomeScreenAPI.add_homescreen_image"
									/>
								</v-col>
							</v-col>
							<v-col cols="4">
								<v-row class="sticky-header">
									<div class="mx-auto mt-3">
										<v-btn class="mr-2 white--text" color="grey" @click="CloseForm">
											Cancel
										</v-btn>
										<v-btn class="mr-2 white--text" color="design" @click="AddEditData">
											{{ edit ? 'Update' : 'Submit' }}
										</v-btn>
									</div>
								</v-row>
							</v-col>
						</v-row>
						<small>*indicates required field</small>
					</v-col>
				</v-row>

			</v-form>
		</v-card-text>
	</v-card>
</template>

<script>
import { map } from 'lodash'
import TagAPI from '@/utils/api/tag'
import BrandAPI from '@/utils/api/brand'
import SellerAPI from '@/utils/api/SellerFormAPI'
import ProductAPI from '@/utils/api/ProductFormAPI'
import HealthconcernAPI from '@/utils/api/healthconcern'
import HomeScreenAPI from '@/utils/api/homescreen'

export default {
	data: () => ({
		ProductAPI: ProductAPI,
		HomeScreenAPI: HomeScreenAPI,
		isValid: false,
		d_tagList: [],
		d_hsnList: [],
		d_labelList: [],
		d_brandList: [],
		d_sellerList: [],
		d_categoryList: [],
		d_subcategoryList: [],
		d_healthconcernList: [],
		payload: {
			product_name: '',
			product_image: '',
			ingredients: '',
			weight: '',
			fat: 'fat',
			protein: 'energy',
			carbohydrates: 'carbohydrates',
			energy: 'energy',
			acidity_as_citric_acid: 'energy',
			sugar: 'energy',
			calcium: 'energy',
			trans_fat: 'energy',
			saturated_fat: 'energy',
			sodium: 'energy',
			citric_acid: 'energy',
			taurine: 'energy',
			caffeine: 'energy',
			inositol: 'energy',
			niacin: 'energy',
			vitamin_b6: 'energy',
			vitamin_b3: 'energy',
			vitamin_b12: 'energy',
			total_fat:'total_fat',
		},
		errorMessages: { product_image: '' },
		rules: {
			required: (value) => !!value || 'This field is required',
			notNegative: (value) => value >= 0 || 'Please enter a non-negative number',
			notNull: (value) => (value !== null && value !== '') || 'This field is required',
		},
	}),
	watch: {
		edit: {
			handler(newVal, oldVal) {
				if (newVal) {
					this.payload = { ...this.payload, ...this.content }
					this.payload.product_id = this.content._id
					// this.payload.selling_price = this.content?.seller_list[0]?.selling_price
					// this.payload.brand_id = this.content?.brand?._id
					// this.payload.seller_id = this.content?.seller_list[0]?.seller?._id
					// Removing unnecessary keys
					delete this.payload.__v
					delete this.payload._id
					delete this.payload.createdAt
					delete this.payload.updatedAt
				} else {
					this.ResetForm()
				}
			},
			immediate: true,
		},
	},
	props: {
		content: { type: Object, default: false },
		edit: { type: Boolean, default: false },
	},
	methods: {
		async DeleteData(itemToDelete) {

try {
	const response = await ProductAPI.deleteAllProductById({
		blog_id: itemToDelete,
	})
	if (response.status.status_code === 0) {
		this.$store.dispatch('ActivateSnackBar', {
			state: true,
			color: 'green darken-4',
			msg: 'Item deleted successfully',
		})
	}
	this.FetchData()
} catch (err) {
	console.log(err)
}
},
		async AddEditData() {
			this.$refs.form.validate()
			const isImagesValid = this.isImagesValidated(['image'])
			console.log('out side of if 123',this.isValid)
			console.log('out -----------------',isImagesValid)
			if (this.isValid && isImagesValid) {
				try {
					if (this.payload?.product_image?.imageUrl) {
					this.payload.product_image = this.payload.product_image.imageUrl
				}
					console.log('in side of if')

					if (this.edit) {
						
						await ProductAPI.updateProduct(this.payload)
						this.$emit('close_edit')
						this.ResetForm()
						this.$emit('change')
						this.$emit('close')
					} else {
						console.log('in side of else if1111111')

						const response = await ProductAPI.addProduct(this.payload)
						console.log('add product', this.payload)
						if (response.data.status.status_code == 1) {
							this.$store.dispatch('ActivateSnackBar', {
								state: true,
								color: 'red darken-4',
								msg: response.data.status.message,
							})
						} else if (response.data.status.status_code == 0) {
							this.$store.dispatch('ActivateSnackBar', {
								state: true,
								color: 'green darken-4',
								msg: response.data.status.message,
							})
							this.ResetForm()
							this.$emit('change')
							this.$emit('close')
						} else {
							this.$store.dispatch('ActivateSnackBar', {
								state: true,
								color: 'red darken-4',
								msg: response.data.status.message,
							})
						}
					}
				} catch (err) {
					console.log(err)
				}
			} else {
				console.log('in side of else')
				this.errorMessages.description = 'This is required'
			}
		},

		isImagesValidated(itemsToValidate) {
			let isValid = true
			map(itemsToValidate, (item) => {
				if (typeof this.payload[item] === 'string') {
					this.errorMessages[item] = this.payload[item] ? '' : 'This is required'
					isValid = isValid && !!this.payload[item]
				} else if (typeof this.payload[item] === 'object') {
					this.errorMessages[item] = this.payload[item] ? '' : 'This is required'
					isValid = isValid && !!this.payload[item]
				}
			})
			return isValid
		},

		ResetForm() {
			this.payload = {
				product_name: 'product_name',
				product_image: '',
				ingredients: 'ingredients',
				weight: 'weight',
				fat: 'fat',
				protein: 'energy',
				carbohydrates: 'carbohydrates',
				energy: 'energy',
				acidity_as_citric_acid: 'energy',
				sugar: 'energy',
				calcium: 'energy',
				trans_fat: 'energy',
				saturated_fat: 'energy',
				sodium: 'energy',
				citric_acid: 'energy',
				taurine: 'energy',
				caffeine: 'energy',
				inositol: 'energy',
				niacin: 'energy',
				vitamin_b6: 'energy',
				vitamin_b3: 'energy',
				vitamin_b12: 'energy',
				total_fat:"total_fat",
			}
			this.$refs?.form?.resetValidation()
		},
		CloseForm() {
			if (this.edit) {
				this.ResetForm()
				this.$emit('close_edit')
			}
			this.$emit('close')
		},
		descriptionHide() {
			console.log('description')
			if (this.payload.description.length) {
				console.log('description1', this.payload.description.length)
				this.errorMessages.description = ''
			}
		},
	},
	mounted() {
		this.$nextTick(async () => {
			await Promise.all([])
		})
	},
}
</script>

<style scoped>
.sticky-header {
	top: 0;
	z-index: 100;
	position: sticky;
}
</style>
